import sys
import time

def jalan_lirik():
    lirik = [
        ("temanku semua pada jahat tante",0.1),
        ("aku lagi susah mereka gak ada",0.1),
        ("coba kalo lagi jayaaaa",0.1),
        ("aku dipuja puja tantee",0.1),
        ("sudah terbiasa terjadi tante",0.1),
        ("teman datang ketika lagi butuh saja",0.1),
        ("coba kalo lagi susahhhh",0.1),
        ("mereka semua menghilanggggg",0.2),
        ("(TANTEEEE)",0.3),
        ("(TANTEEEE)",0.3),
    ]
    
    delay = [1.1, 1.4, 1.3, 1.6, 1.25, 1.1, 1, 1.5, 0.8, 0.7]
    print("~TANTEEE~")
    time.sleep(3)
    for i, (baris_lagu, delay_char) in enumerate(lirik):
        for char in baris_lagu:
            print(char, end='')
            sys.stdout.flush()
            time.sleep(delay_char)
        time.sleep(delay[i])
        print('')
        
    print("//Code By aqila")    
    
jalan_lirik()    
