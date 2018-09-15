#import sys
def func(line):
    n = int(line)
    res = 0

    def func(n):
        count = 0
        while n:
            count += n //5
            n = n//5
        return count

    for i in range(1, n + 1):
        res += func(i)

    return res

if __name__=="__main__":
    m = sys.stdin.readline().strip()
    print func("11")
