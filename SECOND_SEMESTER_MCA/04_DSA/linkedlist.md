# single

``` c
#include <stdio.h>
#include <stdlib.h>
struct node
{

    int data;
    struct node *next;

};

struct node * llcreation(){
    int choice;
    struct node * head = NULL, *newnode , *temp;

    while(choice){
        newnode = (struct node *) malloc (sizeof(struct node));
        printf("enter data\n");
        scanf("%d",&newnode->data);
        newnode->next=0;
        if (head == NULL)
        {
            head = newnode;
            temp = head;
        }else{
            temp->next = newnode;
            temp = newnode;
        }

        printf("do you want add kore\n(0 for no 1 for yes)");
        scanf("%d",&choice);
        
    }

    return head;
}

struct node * deletAtBegining (struct node * head){
    struct node *temp = head;
    head = head->next;
    free(temp);
    return head;
}
struct node * deletAtEnd (struct node * head){
    struct node *temp = head , *prevnode;

    while(temp->next!=0){
        prevnode = temp;
        temp = temp->next;
    }
    prevnode->next = 0;
    free(temp);
    return head;
}
void printlist(struct node * head){
    struct node * temp = head;
    while(temp !=0){
        printf("%d",temp->data);
        temp = temp->next;
    }
}

int main(){
    struct node * head = llcreation();
    head = deletAtBegining(head);
    printf("after delet at begining\n");
    printlist(head);
    printf("\nafter delet at end\n");
    head = deletAtEnd(head);
    printlist(head);
}
```
