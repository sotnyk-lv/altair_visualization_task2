# altair_visualization_task2

## folers: 
```
├───code  
│   ├─── task1.ipynb
│   ├─── task2.ipynb
│   ├─── task3.ipynb
│   ├─── task4.ipynb
│   └─── task5.ipynb
├───data  
│   └─── 2014-2020.xlsx
├───res  
│   ├─── task1_full.png
│   ├─── task2_horizontal.png
│   ├─── task3_2x2.png
│   ├─── task4.png
│   └─── task5.png
└───tests  
    ├─── image results
    └─── some code tests
```
## comments:
### Task 1
- Як змінювалась структура генерації електроенергії за роками?  
![res/task1 full.png](/res/task1_full.png?raw=true)
Важливим фактором для цієї візуалізації є можливість порівняти результати за різні роки.  
Стовпцева діаграма дозволяє непогано досягнути цього.  
Важливим було посортувати категорії за зростанням їхнього вкладу для зручності поріняння.  
- Як залежить споживання електроенергії від дня року та години доби?
![res/task2_horizontal.png](/res/task2_horizontal.png?raw=true)
Для зображення цієї інформації я передав кількість використаної енергії кольором: червоний - більше, зелений - менше, що є досить асоціативним.
На осі Х знаходяться числа року. Кількість днів є досить великою, проте оскільки кольори змінюються досить плавно, то різких змін майже немає, і за рахунок плавного градєнту можна зрозуміти структуру використання енергії.
На візуалізації чітко видно сезонності: тижневі колиання, коливання пір року та добові зміни.
Для агрегації даних я обрав середнє значення по всій вибірці для кожного дня та години.
- Як змінюється генерація електроенергії з різних джерел впродовж доби?
![res/task3_2x2.png](/res/task3_2x2.png?raw=true)
У цьому завданні не потрібно було показувати сезонну зміну, проте добова генерація електроенергії змінюється відносно пір року (особливо Відновлювальні джерела електроенергії).
Тому замість того, щоб усереднювати дані по сезонах чи обмежувати вибірку тільки одним сезоном я надав 4 графіки. 
Всі вони є повноцнними і незалежними, та не мали б відволікати увагу спостерігача, а тільки поглиблювати розуміння даних. 
Іншим можливим варіантом розміщення, який я розглядав (можна побачити результат в папці tests) було розміщення всіх сезонів в 1 ряд. 
Це підкреслювало б зміну виробленої енергії для різних пір року. Проте такий підхід може відволікати спостерігача, адже графіки були б на еликій відстані і знаходення необхідної інформації моглоб займати більше часу.
Оскільки першочерговим було завдання відображення динаміки впродовж доби, я вирішив знехтувати можливістю порівняння міжсезонних змін.
- Як змінюється споживання електроенергії впродовж доби у розрізі місяців року та пір року?
![res/task3_2x2.png](/res/task4.png?raw=true)
Для цієї візуалізації важливими є кольори. Адже даних є досить багато, вони часто накладаються чи перетинаються.
Тому важливим було за допомогою кольору швидко зрозуміти який місяць зображено. Для цього я використав 12 зациклених кольорів, які формують веселку.
У візуалізації зимовим місяцям відповідають сині кольори, весняним - зелені, літо - перехід до жовтого, оранжевого, а осіць - це червоно-рожеві кольори.
Сірий фон дозвоняє краще розрізняти відтінки на контрасті.
- Як змінюється споживання електроенергії впродовж тижня?
- ![res/task3_2x2.png](/res/task5.png?raw=true)
Цей графік є досить простим і прямолінійним. Дані агреговано за днм тижня і усереднено.
