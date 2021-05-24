class Solution {
    public int numRookCaptures(char[][] board) {
        int rrow=0;
        int rcolumn=0;
        int bcolumn=0;
        int brow=0;
        int pcolumn=0;
        int prow=0;
       int count=0;
        int result=0;
        for(int i=0;i<8;i++)
        {
            for(int j=0;j<8;j++)
            {
                if(board[i][j]=='R')
                {
                     rrow=i;
                    rcolumn=j;
                    break;
                }
                   
            }
        }
        boolean left=true;
        boolean top=true;
        for(int i=0;i<8;i++)
        {
            if(left)
            {
                if(board[rrow][i]=='p')
                {
                    count++;
                }
                else if(board[rrow][i]=='B')
                {
                    count=0;
                }
            }
            if(i==rrow)
            {
                if(count>0)
                {
                    result=result+1;
                }
                left=false;
            }
            if(!left)
            {
                 if(board[rrow][i]=='B')
                {
                    break;
                }
                else if(board[rrow][i]=='p')
                {
                    result++;
                    break;
                }
            }
        }
       // System.out.println(result);
        count=0;
        for(int i=0;i<8;i++)
        {
            if(top)
            {
                if(board[i][rcolumn]=='p')
                {
                    count++;
                }
                else if(board[i][rcolumn]=='B')
                {
                    count=0;
                }
                System.out.println(count);
            }
             
            if(i==rcolumn)
            {
                if(count>0)
                {
                    result=result+1;
                }
                top=false;
            }
            if(!top)
            {
                 if(board[i][rcolumn]=='B')
                {
                    break;
                }
                else if(board[i][rcolumn]=='p')
                {
                    result++;
                    break;
                }
            }
        }
         System.out.println(result);
        return result;  
        
    }
}
