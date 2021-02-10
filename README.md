
#include <stdio.h>
#include <stdlib.h>
#include <string.h>
#include <conio.h>

typedef struct ships{
    int ship5[4];
    int ship31[4];
    int ship32[4];
    int ship21[4];
    int ship22[4];
    int ship23[4];
    int ship11[2];
    int ship12[2];
    int ship13[2];
    int ship14[2];
}player;
player p1,p2;

char board1[11][11],board2[11][11];
int play1[10][10],play2[10][10];

char turn_map2(char turn, int x, int y){
    if (turn=='a'){

    }
}

char turn_map_bot(){

}

void get_ships1(){
    printf("Please enter the coordinates at the beginning of your five-box ship.");
    scanf("%d %d",&p1.ship5[0],&p1.ship5[1]);
    printf("Please enter the coordinates at the end of your five-box ship.");
    scanf("%d %d",&p1.ship5[2],&p1.ship5[3]);
    while (p1.ship5[2]-p1.ship5[0]!=4||p1.ship5[3]-p1.ship5[1]!=4){
        printf("not acceptable. enter again.");
        scanf("%d %d",&p1.ship5[0],&p1.ship5[1]);
        scanf("%d %d",&p1.ship5[2],&p1.ship5[3]);
        if (p1.ship5[2]-p1.ship5[0]==4||p1.ship5[3]-p1.ship5[1]==4){
            break;
        }
    }
    printf("Please enter the coordinates at the beginning of your first three-box ship.");
    scanf("%d %d",&p1.ship31[0],&p1.ship31[1]);
    printf("Please enter the coordinates at the end of your first three-box ship.");
    scanf("%d %d",&p1.ship31[2],&p1.ship31[3]);
    while (p1.ship31[2]-p1.ship31[0]!=2||p1.ship31[3]-p1.ship31[1]!=2){
        printf("not acceptable. enter again.");
        scanf("%d %d",&p1.ship31[0],&p1.ship31[1]);
        scanf("%d %d",&p1.ship31[2],&p1.ship31[3]);
        if (p1.ship31[2]-p1.ship31[0]==2||p1.ship31[3]-p1.ship31[1]==2){
            break;
        }
    }
    printf("Please enter the coordinates at the beginning of your second three-box ship.");
    scanf("%d %d",&p1.ship32[0],&p1.ship31[1]);
    printf("Please enter the coordinates at the end of your second three-box ship.");
    scanf("%d %d",&p1.ship32[2],&p1.ship32[3]);
    while (p1.ship32[2]-p1.ship32[0]!=2||p1.ship32[3]-p1.ship32[1]!=2){
        printf("not acceptable. enter again.");
        scanf("%d %d",&p1.ship32[0],&p1.ship32[1]);
        scanf("%d %d",&p1.ship32[2],&p1.ship32[3]);
        if (p1.ship32[2]-p1.ship32[0]==2||p1.ship32[3]-p1.ship32[1]==2){
            break;
        }
    }
    printf("Please enter the coordinates at the beginning of your first two-box ship.");
    scanf("%d %d",&p1.ship21[0],&p1.ship21[1]);
    printf("Please enter the coordinates at the end of your first two-box ship.");
    scanf("%d %d",&p1.ship21[2],&p1.ship21[3]);
    while (p1.ship21[2]-p1.ship21[0]!=1||p1.ship21[3]-p1.ship21[1]!=1){
        printf("not acceptable. enter again.");
        scanf("%d %d",&p1.ship21[0],&p1.ship21[1]);
        scanf("%d %d",&p1.ship21[2],&p1.ship21[3]);
        if (p1.ship21[2]-p1.ship21[0]==1||p1.ship21[3]-p1.ship21[1]==1){
            break;
        }
    }
    printf("Please enter the coordinates at the beginning of your second two-box ship.");
    scanf("%d %d",&p1.ship22[0],&p1.ship22[1]);
    printf("Please enter the coordinates at the end of your second two-box ship.");
    scanf("%d %d",&p1.ship22[2],&p1.ship22[3]);
    while (p1.ship22[2]-p1.ship22[0]!=1||p1.ship22[3]-p1.ship22[1]!=1){
        printf("not acceptable. enter again.");
        scanf("%d %d",&p1.ship22[0],&p1.ship22[1]);
        scanf("%d %d",&p1.ship22[2],&p1.ship22[3]);
        if (p1.ship22[2]-p1.ship22[0]==1||p1.ship22[3]-p1.ship22[1]==1){
            break;
        }
    }
    printf("Please enter the coordinates at the beginning of your third two-box ship.");
    scanf("%d %d",&p1.ship23[0],&p1.ship23[1]);
    printf("Please enter the coordinates at the end of your third two-box ship.");
    scanf("%d %d",&p1.ship23[2],&p1.ship23[3]);
    while (p1.ship23[2]-p1.ship23[0]!=1||p1.ship23[3]-p1.ship23[1]!=1){
        printf("not acceptable. enter again.");
        scanf("%d %d",&p1.ship23[0],&p1.ship23[1]);
        scanf("%d %d",&p1.ship21[2],&p1.ship21[3]);
        if (p1.ship23[2]-p1.ship23[0]==1||p1.ship23[3]-p1.ship23[1]==1){
            break;
        }
    }
    printf("Please enter the coordinates of your first one-box ship.");
    scanf("%d %d",&p1.ship11[0],&p1.ship11[1]);
    printf("Please enter the coordinates  of your second one-box ship.");
    scanf("%d %d",&p1.ship12[0],&p1.ship12[1]);
    printf("Please enter the coordinates of your third one-box ship.");
    scanf("%d %d",&p1.ship13[0],&p1.ship13[1]);
    printf("Please enter the coordinates of your fourth one-box ship.");
    scanf("%d %d",&p1.ship14[0],&p1.ship14[1]);
}
void get_ships2(){
    printf("Please enter the coordinates at the beginning of your five-box ship.");
    scanf("%d %d",&p2.ship5[0],&p2.ship5[1]);
    printf("Please enter the coordinates at the end of your five-box ship.");
    scanf("%d %d",&p2.ship5[2],&p2.ship5[3]);
    while (p2.ship5[2]-p2.ship5[0]!=4||p2.ship5[3]-p2.ship5[1]!=4){
        printf("not acceptable. enter again.");
        scanf("%d %d",&p2.ship5[0],&p2.ship5[1]);
        scanf("%d %d",&p2.ship5[2],&p2.ship5[3]);
        if (p2.ship5[2]-p2.ship5[0]==4||p2.ship5[3]-p2.ship5[1]==4){
            break;
        }
    }
    printf("Please enter the coordinates at the beginning of your first three-box ship.");
    scanf("%d %d",&p2.ship31[0],&p2.ship31[1]);
    printf("Please enter the coordinates at the end of your first three-box ship.");
    scanf("%d %d",&p2.ship31[2],&p2.ship31[3]);
    while (p2.ship31[2]-p2.ship31[0]!=2||p2.ship31[3]-p2.ship31[1]!=2){
        printf("not acceptable. enter again.");
        scanf("%d %d",&p2.ship31[0],&p2.ship31[1]);
        scanf("%d %d",&p2.ship31[2],&p2.ship31[3]);
        if (p2.ship31[2]-p2.ship31[0]==2||p2.ship31[3]-p2.ship31[1]==2){
            break;
        }
    }
    printf("Please enter the coordinates at the beginning of your second three-box ship.");
    scanf("%d %d",&p2.ship32[0],&p2.ship31[1]);
    printf("Please enter the coordinates at the end of your second three-box ship.");
    scanf("%d %d",&p2.ship32[2],&p2.ship32[3]);
    while (p2.ship32[2]-p2.ship32[0]!=2||p2.ship32[3]-p2.ship32[1]!=2){
        printf("not acceptable. enter again.");
        scanf("%d %d",&p2.ship32[0],&p2.ship32[1]);
        scanf("%d %d",&p2.ship32[2],&p2.ship32[3]);
        if (p2.ship32[2]-p2.ship32[0]==2||p2.ship32[3]-p2.ship32[1]==2){
            break;
        }
    }
    printf("Please enter the coordinates at the beginning of your first two-box ship.");
    scanf("%d %d",&p2.ship21[0],&p2.ship21[1]);
    printf("Please enter the coordinates at the end of your first two-box ship.");
    scanf("%d %d",&p2.ship21[2],&p2.ship21[3]);
    while (p2.ship21[2]-p2.ship21[0]!=1||p2.ship21[3]-p2.ship21[1]!=1){
        printf("not acceptable. enter again.");
        scanf("%d %d",&p2.ship21[0],&p2.ship21[1]);
        scanf("%d %d",&p2.ship21[2],&p2.ship21[3]);
        if (p2.ship21[2]-p2.ship21[0]==1||p2.ship21[3]-p2.ship21[1]==1){
            break;
        }
    }
    printf("Please enter the coordinates at the beginning of your second two-box ship.");
    scanf("%d %d",&p2.ship22[0],&p2.ship22[1]);
    printf("Please enter the coordinates at the end of your second two-box ship.");
    scanf("%d %d",&p2.ship22[2],&p2.ship22[3]);
    while (p2.ship22[2]-p2.ship22[0]!=1||p2.ship22[3]-p2.ship22[1]!=1){
        printf("not acceptable. enter again.");
        scanf("%d %d",&p2.ship22[0],&p2.ship22[1]);
        scanf("%d %d",&p2.ship22[2],&p2.ship22[3]);
        if (p2.ship22[2]-p2.ship22[0]==1||p2.ship22[3]-p2.ship22[1]==1){
            break;
        }
    }
    printf("Please enter the coordinates at the beginning of your third two-box ship.");
    scanf("%d %d",&p1.ship23[0],&p1.ship23[1]);
    printf("Please enter the coordinates at the end of your third two-box ship.");
    scanf("%d %d",&p1.ship23[2],&p1.ship23[3]);
    while (p1.ship23[2]-p1.ship23[0]!=1||p1.ship23[3]-p1.ship23[1]!=1){
        printf("not acceptable. enter again.");
        scanf("%d %d",&p1.ship23[0],&p1.ship23[1]);
        scanf("%d %d",&p1.ship21[2],&p1.ship21[3]);
        if (p1.ship23[2]-p1.ship23[0]==1||p1.ship23[3]-p1.ship23[1]==1){
            break;
        }
    }
    printf("Please enter the coordinates of your first one-box ship.");
    scanf("%d %d",&p2.ship11[0],&p2.ship11[1]);
    printf("Please enter the coordinates  of your second one-box ship.");
    scanf("%d %d",&p2.ship12[0],&p2.ship13[0],&p1.ship13[1]);
    printf("Please enter the coordinates of your fourth one-box ship.");
    scanf("%d %d",&p2.ship14[0],&p2.ship14[1]);
}
void turn_operation(){

}

int main() {
    printf("Hello, lets have fun during this battle:)!\n");

    return 0;
}
