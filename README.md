# Battleship Game
This is a C++ implementation of the classic Battleship game. Two players place ships on a 10x10 grid and take turns firing at each other's ships.

## Rules
Each player places 5 ships on their grid:
+ 1 x 4 cell ship
+ 2 x 3 cell ships
+ 3 x 2 cell ships
+ 4 x 1 cell ships

Players alternate turns firing at a grid coordinate

If a ship is hit, the player marks it on their tracking grid

The first player to sink all enemy ships wins

## Code Overview
The core logic is in main():

+ a[][] - Player 1's ocean grid
+ pc[][] - Player 2's ocean grid
+ pcn[][] - Player 2's tracking grid

Ships are pre-populated for simplicity.

Game loop:

1. Player 1 fires shot at pc[][]
  + Check for hit or miss and mark pcn[][]
2. Check if Player 2 ships sunk. If yes, Player 1 wins
3. Player 2 fires shot at a[][]
  + Check for hit or miss
4. Check if Player 1 ships sunk. If yes, Player 2 wins
5. Repeat turns until a player wins

win() function checks if all ships sunk by analyzing the ocean grid.

Input validation ensures shots are at unused spots.

## Usage

+ Compile and run Battleship.cpp
+ Follow prompts to play

## Enhancements
+ Allow players to position their own ships
+ Improve input validation
+ Add difficulty levels
+ Enhance UI and graphics

## Conclusion
This demonstrates a basic C++ implementation of the game using 2D arrays, functions, and other language features.

Let me know if any part of the code needs further explanation!








# Fundamentals-Computer-and-Programming
Fourth Project Computer and Programming Fundamentals

More info in pdf file Attached


https://en.wikipedia.org/wiki/Battleship_(game)

https://battleship-game.org/en/

https://telegram.me/nabardbot





قوانین بازی

1. در حین بازی، هیچ کدام از بازیکنان محل کشتی های رقیبشان را نمی بینید.

1۰ است. × 2. ابعاد نقشه ی بازی 1۰


3. هر بازیکن 1۰ کشتی از قرار زیر دارد:
نام طول تعداد
ناو 1 4
رزم ناو 2 3
ناوشکن 3 2
زیر دریایی 4 1

4. هر کشتی می تواند به صورت اعمودی و یا افقی در صفحه قرار بگیرد.

5. هر کشتی به اندازه ی یک خانه اطراف خود حریم دارد و کشتی دیگری نباید در آن فضا قرار بگیرد.

6. هر بازیکن در نوبت خود به یکی از خانه های نقشه ی حریف شلیک می کند و مادامی که شلیکش یک شلیک موفق باشد

تصویر 1: نمایش حریم ناو
پروژه ی چهارم مبانی برنامه سازی
کشتی جنگی) ) Battleship بازی
می تواند به شلیک کردن ادامه دهد.

7. بازیکن این امکان را دارد که خودش کشتی هایش را در صفحه بچیند.

8. پس از هر شلیک موفق، خانه هایی که ممکن نیست ادامه ی کشت ی ی اصابت شده در آن ها باشد در نقشه مشخص
می شوند. این خانه ها بخشی از حریم کشتی هستند که در راستای شمالی-جنوبی و یا شرقی-غربی، که احتمال دارد ادامه ی
کشتی در آن جا باشد، قرار ندارند. برای روشن شدن موضوع تصویر زیر را ببینید. در حقیقت این خانه ها به اعنوان خانه هایی
که مورد اصابت قرار گرفته اند ولی خالی بودند مشخص می شوند.

9. بازی تا جایی ادامه پیدا می کند که یکی از بازیکنان تمامی کشتی های بازیکن دیگر را غرق کرده باشد. در انتهای بازی و با
ااعلم برنده ، بازنده از محل کشتی های برنده آگاه می شود. (هر دو نقشه به صورت کامل نشان داده می شوند.)




