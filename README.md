# SAT Raw Score Converter
📝✏️✎✐✏︎ SAT Scores typically vary by difficulty, in other words, each and every test utilizes a different scoring system. This is just an approximation of what score you'll get. :)

This is the table I used for the convertion:

![SAT table](https://github.com/jeremygautama/SAT-Raw-Score-Converter/blob/main/images/SATTable.png)

## Code (for Python 3)
```bash
readingRawScore = int(input("Input your Reading raw score (0-52): "))
if (0 <= readingRawScore <= 52):
    writingRawScore = int(input("Input your Writing and Language raw score (0-44): "))
    if (0 <= writingRawScore <= 44):
        noCalcRawScore = int(input("Input your Math (NO calculator) raw score (0-20): "))
        if (0 <= noCalcRawScore <= 20):
            calcRawScore = int(input("Input your Math (calculator OK) raw score (0-38): "))
            if (0 <= calcRawScore <= 38):

                print("-----------------------------")
                
                #Calculating the MATH RAW score to the MATH SAT score
                mathRawScore = noCalcRawScore + calcRawScore
                #Raw score: 0   1   2   3   4   5   6   7   8   9   10  11  12  13  14  15  16  17  18  19  20  21  22  23  24  25  26  27  28  29  30  31  32  33  34  35  36  37  38  39  40  41  42  43  44  45  46  47  48  49  50  51  52  53  54  55  56  57  58
                mathSAT = [200,200,210,230,250,270,280,300,320,340,350,360,370,390,410,420,430,450,460,470,480,490,500,510,520,530,540,550,560,570,580,590,600,600,610,620,630,640,650,660,670,680,690,700,710,710,720,730,730,740,750,750,760,770,780,790,790,800,800]
                print("Your SAT Math score is:", mathSAT[mathRawScore])

                #Calculating the READING RAW score to the READING SAT score
                #Raw score:    0  1  2  3  4  5  6  7  8  9 10 11 12 13 14 15 16 17 18 19 20 21 22 23 24 25 26 27 28 29 30 31 32 33 34 35 36 37 38 39 40 41 42 43 44 45 46 47 48 49 50 51 52
                readingSAT = [10,10,10,11,12,13,14,15,16,16,17,18,18,19,20,20,21,21,22,22,23,23,23,24,24,25,25,26,26,27,27,28,28,28,29,29,30,30,31,31,32,32,33,33,34,35,35,36,37,38,39,39,40]
                print("Your SAT Reading score is:", readingSAT[readingRawScore]*10)

                #Calculating the WRITING AND LANGUAGE RAW score to the WRITING AND LANGUAGE SAT score
                #Raw score:    0  1  2  3  4  5  6  7  8  9 10 11 12 13 14 15 16 17 18 19 20 21 22 23 24 25 26 27 28 29 30 31 32 33 34 35 36 37 38 39 40 41 42 43 44
                writingSAT = [10,10,10,10,11,12,13,14,15,16,16,17,18,19,19,20,21,22,23,23,24,24,25,26,26,27,27,28,29,29,30,31,31,32,32,33,33,34,35,36,37,37,38,39,40]
                print("Your SAT Writing and Language score is:", writingSAT[writingRawScore]*10)

                #Calculating the final score
                english = (readingSAT[readingRawScore] + writingSAT[writingRawScore]) * 10
                math = mathSAT[mathRawScore]
                finalScore = english + math
                print("-----------------------------")
                print("Your SAT Score is:",finalScore)
                print("-----------------------------")


            else:
                print("Error! Enter a score between 0-38! :)")
        else: 
            print("Error! Enter a score between 0-20! :)")
    else:
        print("Error! Enter a score between 0-44! :)")
else:
    print("Error! Enter a score between 0-52! :)")
```

## Contributing
✅ Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate. 👌

1. Fork it (<https://github.com/jeremygautama/SAT-Raw-Score-Converter/fork>)
2. Create your feature branch (`git checkout -b feature/fooBar`)
3. Commit your changes (`git commit -am 'Add some fooBar'`)
4. Push to the branch (`git push origin feature/fooBar`)
5. Create a new Pull Request

## Support
⭐️ Your **star** means so much. Thank You!

📢 Help spread the word!!!

## Author
👤 Jeremy Gautama 

## Contact
🥨 If you have any questions, feel free to [email](mailto:mail.jeremygautama@gmail.com) me or to visit my [website](https://jeremygautama.github.io). Thanks!

