# Ex17 AVL Tree – Rotation
## DATE: 29/03/2025
## AIM:
To write a C function to perform right rotation in an AVL Tree.

## Algorithm
1. Start 
2. Set y to the left child of x. 
3. Set the left child of x to be the right child of y. 
4. Set the right child of y to be x. 
5. Update the height of x and y. 
6. Return y as the new root after rotation. 
7. End 
## Program:
```

Program to perform right rotation in AVL Tree

Developed by: Shanmuga Vasanth M

RegisterNumber: 212223040191
```
```
typedef struct node 
{ 
int data; 
struct node *left,*right; 
int ht; 
}node; 
node *insert(node *,int); 
//node *Delete(node *,int); 
void preorder(node *); 
//void inorder(node *); 
int height( node *); 
node *rotateright(node *); 
node *rotateleft(node *); 
node *RR(node *); 
node *LL(node *); 
node *LR(node *); 
node *RL(node *); 
*/ 
node * rotateright(node *x) 
{ 
node *y; 
y=x->left; 
x->left=y->right; 
y->right=x; 
  
  
x->ht=height(x); 
y->ht=height(y); 
return(y); 
}
```

## Output:

![437418378-f45d6171-60c8-4445-b622-e840c16b6b49](https://github.com/user-attachments/assets/313b875f-e893-4f4d-a10b-d27e3774be52)


## Result:

Thus, the function to perform right rotation in an AVL Tree is implemented successfully.
