# Drawing-book-Hackerrank-problem

def pageCount(n, p):
    countf=0
    countb=0
    i=1
    while i!=p:
        if i%2!=0:
            countf+=1
        i+=1
    i=n
    while i!=p:
        if i%2==0:
            countb+=1
        i-=1
    return min(countf,countb)        
                
            
        
if __name__ == '__main__':
    fptr = open(os.environ['OUTPUT_PATH'], 'w')

    n = int(input().strip())

    p = int(input().strip())

    result = pageCount(n, p)

    fptr.write(str(result) + '\n')

    fptr.close()
