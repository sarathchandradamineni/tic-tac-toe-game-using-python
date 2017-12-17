# tic-tac-toe-game-using-python
l=[' ',' ',' ',' ',' ',' ',' ',' ',' ']
def board():
    print("        |           |           ")
    print("  %s     |    %s      |    %s     " % (l[0], l[1], l[2]))
    print("________|___________|__________ ")
    print("        |           |           ")
    print("  %s     |    %s      |    %s     " % (l[3], l[4], l[5]))
    print("________|___________|__________ ")
    print("        |           |           ")
    print("  %s     |    %s      |    %s     " % (l[6], l[7], l[8]))
    print("        |           |           ")
from IPython.display import clear_output
def inputgame():
    global l
    for i in range(0,5):
        if l[0] == l[3] == l[6] and l[0] != ' ':
            if l[0] == 'x':
                print('player one won')
                break
            elif l[0] == 'o':
                print('player two won')
                break
        elif l[1] == l[4] == l[7] and l[1] !=' ':
            if l[4] == 'x':
                print('player one won')
                break
            elif l[1] == 'o':
                print('player two won')
                break
        elif l[2] == l[5] == l[8] and l[2] != ' ':
            if l[2] == 'x':
                print('player one won')
                break
            elif l[2] == 'o':
                print('player two won')
                break
        elif l[0] == l[1] == l[2] and l[0] != ' ':
            if l[0] == 'x':
                print('player one won')
                break
            elif l[0]=='o':
                print('player two won')
                break
        elif l[3] == l[4] == l[5] and l[3] != ' ':
            if l[4] == 'x':
                print('player one won')
                break
            elif l[3] == 'o' :
                print('player two won')
                break
        elif l[6] == l[7] == l[8] and l[6] != ' ':
            if l[6] == 'x':
                print('player one won')
                break
            elif l[6] == 'o' :
                print('player two won')
                break
        elif l[0] == l[4] == l[8] and l[0] != ' ':
            if l[0] == 'x':
                print('player one won')
                break
            elif l[0] == 'o':
                print('player two won')
                break
        elif l[6] == l[4] == l[2] and l[6] != ' ':
            if l[6] == 'x':
                print('player one won')
                break
            elif l[6] == 'o' :
                print('player two won')
                break
        else:
            count = 0
            for j in range(0,9):
                if l[j] == 'x' or l[j] == 'o' :
                    count+=1
        if count == 9 :
            print("match tied")
            break
        print("player 1 attempt")
        s1 = input()
        clear_output()
        if l[(s1 - 1)] == ' ':
            l[(s1 - 1)] = 'x'
        else:
            board()
            ff=0
            while ff  == 0:
                print("invalid choice aldready entered at position %s"%(s1))
                print("enter at valid position")
                print("player one attempt")
                s1 = input()
                if l[(s1-1)] == ' ':
                    ff+=1
                    l[(s1-1)] = 'x'
            clear_output()
        board()
        if l[0] == l[3] == l[6] and l[0] != ' ':
            if l[0] == 'x':
                print('player one won')
                break
            elif l[0] == 'o':
                print('player two won')
                break
        elif l[1] == l[4] == l[7] and l[1] !=' ':
            if l[4] == 'x':
                print('player one won')
                break
            elif l[1] == 'o':
                print('player two won')
                break
        elif l[2] == l[5] == l[8] and l[2] != ' ':
            if l[2] == 'x':
                print('player one won')
                break
            elif l[2] == 'o':
                print('player two won')
                break
        elif l[0] == l[1] == l[2] and l[0] != ' ':
            if l[0] == 'x':
                print('player one won')
                break
            elif l[0]=='o':
                print('player two won')
                break
        elif l[3] == l[4] == l[5] and l[3] != ' ':
            if l[4] == 'x':
                print('player one won')
                break
            elif l[3] == 'o' :
                print('player two won')
                break
        elif l[6] == l[7] == l[8] and l[6] != ' ':
            if l[6] == 'x':
                print('player one won')
                break
            elif l[6] == 'o' :
                print('player two won')
                break
        elif l[0] == l[4] == l[8] and l[0] != ' ':
            if l[0] == 'x':
                print('player one won')
                break
            elif l[0] == 'o':
                print('player two won')
                break
        elif l[6] == l[4] == l[2] and l[6] != ' ':
            if l[6] == 'x':
                print('player one won')
                break
            elif l[6] == 'o' :
                print('player two won')
                break
        else:
            count = 0
            for j in range(0,9):
                if l[j] == 'x' or l[j] == 'o' :
                    count+=1
        if count == 9 :
            print("match tied")
            break
        print("player 2 attempt")
        s2 = input()
        clear_output()
        if l[(s2 - 1)] == ' ':
            l[(s2 - 1)] = 'o'
        else:
            board()
            fff=0
            while fff  == 0:
                print("invalid choice aldready entered at position %s"%(s2))
                print("enter at valid position")
                print("player two attempt")
                s2 = input()
                if l[(s2-1)] == ' ':
                    fff+=1
                    l[(s2-1)] = 'o'
            clear_output()
        board()
    l = [' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ']

inputgame()
