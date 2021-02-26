CONSOLE_CURSOR_INFO cursor_info = {1, 0}; 

SetConsoleCursorInfo(GetStdHandle(STD_OUTPUT_HANDLE), &cursor_info);

}

 

//把第y行，[x1, x2) 之间的坐标填充为 ch

void drawRow(int y, int x1, int x2, char ch)

{

SetPos(x1,y);

for(int i = 0; i <= (x2-x1); i++)

cout<<ch;

}
