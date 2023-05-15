#### ApiMain15.java
```java
package jp.kronos.main;

import java.util.InputMismatchException;
import java.util.Random;
import java.util.Scanner;

public class ApiMain15 {

    public static void main(String[] args) {
        String[] signs = {"グー", "チョキ", "パー"};
        
        Scanner scan = new Scanner(System.in);
        System.out.println("0:グー、1:チョキ、2:パー");
        
        // プレイヤーの手を入力してもらう
        int player = -1;
        try {
            player = scan.nextInt();
        } catch (InputMismatchException e) {
            System.out.println("入力値が不正です。");
            return;
        }
        
        if (!(player >= 0 && player <= 2)) {
            System.out.println("0～2の数値を入力してください。");
            return;
        }
        
        // コンピュータの手をランダムに決める
        int pc = new Random().nextInt(3);
        
        // それぞれの手を出力する
        System.out.println("PLAYER: " + signs[player]);
        System.out.println("COMPUTER: " + signs[pc]);
        
        // 結果を表示する
        if ((player == 0 && pc == 1) || (player == 1 && pc == 2) || (player == 2 && pc == 0)) {
            System.out.println("YOU WIN!");
        } else if ((player == 0 && pc == 2) || (player == 1 && pc == 0) || (player == 2 && pc == 1)) {
            System.out.println("YOU LOSE!");
        } else {
            System.out.println("DRAW!");
        }
    }

}
```
