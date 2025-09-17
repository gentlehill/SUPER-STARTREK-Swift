# 「BASIC版 SUPER STARTREK」Swift移植版
- macOS ARM CLI Only.

## 概要
SUPER STARTREK - MAY 16,1978版をベースに移植してます

```
10 REM SUPER STARTREK - MAY 16,1978 - REQUIRES 24K MEMORY
30 REM
40 REM ****        **** STAR TREK ****        ****
50 REM **** SIMULATION OF A MISSION OF THE STARSHIP ENTERPRISE,
60 REM **** AS SEEN ON THE STAR TREK TV SHOW.
70 REM **** ORIGIONAL PROGRAM BY MIKE MAYFIELD, MODIFIED VERSION
80 REM **** PUBLISHED IN DEC'S "101 BASIC GAMES", BY DAVE AHL.
90 REM **** MODIFICATIONS TO THE LATTER (PLUS DEBUGGING) BY BOB
100 REM *** LEEDOM - APRIL & DECEMBER 1974,
110 REM *** WITH A LITTLE HELP FROM HIS FRIENDS . . .
120 REM *** COMMENTS, EPITHETS, AND SUGGESTIONS SOLICITED --
130 REM *** SEND TO:  R. C. LEEDOM
140 REM ***           WESTINGHOUSE DEFENSE & ELECTRONICS SYSTEMS CNTR.
150 REM ***           BOX 746, M.S. 338
160 REM ***           BALTIMORE, MD  21203
170 REM ***
180 REM *** CONVERTED TO MICROSOFT 8 K BASIC 3/16/78 BY JOHN GORDERS
190 REM *** LINE NUMBERS FROM VERSION STREK7 OF 1/12/75 PRESERVED AS
200 REM *** MUCH AS POSSIBLE WHILE USING MULTIPLE STATEMENTS PER LINE
205 REM *** SOME LINES ARE LONGER THAN 72 CHARACTERS; THIS WAS DONE
210 REM *** BY USING "?" INSTEAD OF "PRINT" WHEN ENTERING LINES
```

* 参考URL: [http://www.vintage-basic.net/bcg/superstartrek.bas](http://www.vintage-basic.net/bcg/superstartrek.bas)
* 参考URL: [https://en.wikipedia.org/wiki/Star_Trek_(1971_video_game)](https://en.wikipedia.org/wiki/Star_Trek_(1971_video_game))
* 参考URL: [https://ja.wikipedia.org/wiki/%E3%82%B9%E3%82%BF%E3%83%BC%E3%83%88%E3%83%AC%E3%83%83%E3%82%AF_(%E3%83%9E%E3%82%A4%E3%82%B3%E3%83%B3%E3%82%B2%E3%83%BC%E3%83%A0)](https://ja.wikipedia.org/wiki/%E3%82%B9%E3%82%BF%E3%83%BC%E3%83%88%E3%83%AC%E3%83%83%E3%82%AF_(%E3%83%9E%E3%82%A4%E3%82%B3%E3%83%B3%E3%82%B2%E3%83%BC%E3%83%A0))

## 使い方

* ターミナルで使用します。
* 可能な限り、オリジナルコードを尊重して移植してます。<br>オリジナル版同様の挙動だと思います。
* 別プログラムで提供されていた「説明書」を同梱しています。
* 3字コマンドが使い難かったので、1字コマンドを使えるようにしています。
* 残り宇宙暦が無かったので、TIME LEFTとして、追加しております。

***
```

              THE USS ENTERPRISE --- NCC-1701

                              ,------*------,
              ,-------------   '---  ------'
               '-------- --'      / /
                   ,---' '-------/ /--,
                    '----------------'






YOUR ORDERS ARE AS FOLLOWS:
--------------------------
 DESTROY THE 15 KLINGON WARSHIPS WHICH HAVE INVADED
 THE GALAXY BEFORE THEY CAN ATTACK FEDERATION HEADQUARTERS
 ON STARDATE 2130. THIS GIVES YOU 30 DAYS. THERE ARE
 4 STARBASES IN THE GALAXY FOR RESUPPLYING YOUR SHIP.

ARE YOU READY TO ACCEPT COMMAND ('N' FOR INSTRUCTIONS):
```
***
```
5|          *                     |5        PHOTON TORPEDOES   10
6|                                |6        TOTAL ENERGY       3000
7|  *                      <E>    |7        SHIELDS            0
8|                                |8        KLINGONS REMAINING 15
 +--1---2---3---4---5---6---7---8-+         TIME LEFT          30.0

COMMAND: n

COURSE (0-9): 4.8
WARP FACTOR (0-8): 0.5

 +--1---2---3---4---5---6---7---8-+
1|  *       *                     |1        STARDATE           2100.5
2|                                |2        CONDITION          GREEN
3|         <E>      *           * |3        QUADRANT           1,1
4|  *                             |4        SECTOR             3,3
5|          *                     |5        PHOTON TORPEDOES   10
6|                                |6        TOTAL ENERGY       2986
7|  *                             |7        SHIELDS            0
8|                                |8        KLINGONS REMAINING 15
 +--1---2---3---4---5---6---7---8-+         TIME LEFT          29.5

COMMAND:
```
***
```
5|          *                     |5        PHOTON TORPEDOES   10
6|                                |6        TOTAL ENERGY       2986
7|  *                             |7        SHIELDS            0
8|                                |8        KLINGONS REMAINING 15
 +--1---2---3---4---5---6---7---8-+         TIME LEFT          29.5

COMMAND:

ENTER ONE OF THE FOLLOWING:
--------------------------
  NAV | N  (TO SET COURSE)
  SRS | S  (FOR SHORT RANGE SENSOR SCAN)
  LRS | L  (FOR LONG RANGE SENSOR SCAN)
  PHA | P  (TO FIRE PHASERS)
  TOR | T  (TO FIRE PHOTON TORPEDOES)
  SHE | E  (TO RAISE OR LOWER SHIELDS)
  DAM | D  (FOR DAMAGE CONTROL REPORTS)
  COM | C  (TO CALL ON LIBRARY-COMPUTER)
  XXX | X  (TO RESIGN YOUR COMMAND)
  INS | I  (INSTRUCTIONS FOR 'SUPER STAR TREK')

COMMAND:
```
***
```
COMMAND: i

          *************************************
          *                                   *
          *                                   *
          *      * * SUPER STAR TREK * *      *
          *                                   *
          *                                   *
          *************************************

DO YOU NEED INSTRUCTIONS (Y/N): y

      INSTRUCTIONS FOR 'SUPER STAR TREK'

1. WHEN YOU SEE \COMMAND ?\ PRINTED, ENTER ONE OF THE LEGAL
     COMMANDS (NAV,SRS,LRS,PHA,TOR,SHE,DAM,COM, OR XXX).
2. IF YOU SHOULD TYPE IN AN ILLEGAL COMMAND, YOU'LL GET A SHORT
     LIST OF THE LEGAL COMMANDS PRINTED OUT.
3. SOME COMMANDS REQUIRE YOU TO ENTER DATA (FOR EXAMPLE, THE
     'NAV' COMMAND COMES BACK WITH 'COURSE (1-9) ?'.)  IF YOU
     TYPE IN ILLEGAL DATA (LIKE NEGATIVE NUMBERS), THAN COMMAND
     WILL BE ABORTED

```
***

## Changelog

| Date       | Ver   | Log      | OS                    | Compiler           |
| :--------- | :---- | :------- | :-------------------- | :----------------- |
| 2025-09-17 | 0.0.1 | Compiled | macOS Sequoia 15.7 (24G222) | Xcode 16.4 Swift6 |


## Licenses
原作者、著作権者に帰属します
