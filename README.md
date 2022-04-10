# Validate-Expression
ID:6621

The program must accept three positive integers interlaced with two operators (=, +, -, * and %) as the input. The program must print Valid if the expression is valid (RHS = LHS). Else the program must print Invalid as the output. 

Example 
Input/Output 1: 
Input: 5+2=7 
Output: Valid 
Example 
Input/Output 2: 
Input: 2=12-10 
Output: Valid 
Example 
Input/Output 3: 
Input: 11=11=11 
Output: Valid 
Example 
Input/Output 4: 
Input: 6=6=8 
Output: Invalid

Solution:

#include<stdio.h>

#include<stdlib.h>

int main()

{
    
    int a, b, c;
    
    char d, e;
    
    scanf("%d%c%d%c%d", &a,&d,&b,&e,&c);
    
    if(d=='=' && e=='=')
    
    {
        
        if((a==b)&&(b==c))
        
        {
         
         printf("Valid");
        
        }
        
        else
        
        {
            
            printf("Invalid");
        
        }
    
    }
    
    else if(d=='+' &&  e=='=')
    
    {
        
        if(a+b==c)
        
        {
           
           printf("Valid");
        
        }
        
        else
        
        {
            
            printf("Invalid");
        
        }
    
    }
    
    else if(d=='=' && e=='+')
    
    {
        
        if(a==b+c)
        
        {
            
            printf("Valid");
        
        }
        
        else
        
        {
            
            printf("Invalid");
        
        }
    
    }
    
    else if(d=='-' && e=='=')
    
    {
        
        if(a-b==c)
        
        {
            
            printf("Valid");
        
        }
        
        else
        
        {
           
           printf("Invalid");
        
        }
    
    }
    
    else if(d=='=' && e=='-')
    
    {
        
        if(a==b-c)
        
        {
            
            printf("Valid");
        
        }
        
        else
        
        {
            
            printf("Invalid");
        
        }
    
    }
    
    else if(d=='*' && e=='=')
    
    {
        
        if(a*b==c)
        
        {
            
            printf("Valid");
        
        }
        
        else
        {
            
            printf("Invalid");
        
        }
    
    }
    
    else if(d=='=' && e=='*')
    
    {
        
        if(a==b*c)
        
        {
            
            printf("Valid");
        
        }
        
        else
        {
            
            printf("Invalid");
        
        }
    
    }
    
    else if(d=='%' && e=='=')
    
    {
        
        if(a%b==c)
        
        {
            
            printf("Valid");
        
        }
        
        else
        {
            
            printf("Invalid");
        
        }
    
    }
    
    else if(d=='=' && e=='%')
    
    {
        
        if(a==b%c)
        
        {
            
            printf("Valid");
        
        }
        
        else
        
        {
            
            printf("Invalid");
        
        }
    
    }
    
    return 0;
}
