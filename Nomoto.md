## 大工が家を作るアプリケーションを作ろう
&nbsp;&nbsp;&nbsp;&emsp;&emsp;▲   
&emsp;&emsp;▲▼▲  
&nbsp;&emsp;▲▼▲▼▲   
&nbsp;&emsp;|&emsp;&emsp;&emsp;|   
&nbsp;&emsp;|&emsp;&emsp;&emsp;|   
□□□□□□□

## Q1土台メソッド・壁メソッド・屋根メソッドのある家クラスを作成せよ。
なお建設出来る家の数は5軒までとする。  
■一般クラス:House  
<フィールド変数>  
建設した家の軒数:nouseNum  
屋根:roof  
壁 :wall  
土台:fandation  
<メソッド>  
public void makeFoundation(){  
		//土台を作るメソッド  
		//1回土台を作るごとに、フィールドのfondationに文字列"□□□□□□□"を追加する。  		
	}  
public void makeWall(){  
		//壁を作るメソッド  
		//1回壁を作るごとに、フィールドのwallに文字列"&nbsp;&emsp;|&emsp;&emsp;&emsp;|&nbsp;&emsp;"を二段追加する。  
		}  
public void makeRoof(){  
		//屋根を作るメソッド  
		//1回屋根を作るごとに、フィールドのroofに下記の三段の文字列を追加する。  
		// "&nbsp;&nbsp;&nbsp;&emsp;&emsp;▲&nbsp;&nbsp;&nbsp;&emsp;&emsp;"  
		// "&emsp;&emsp;▲▼▲&emsp;&emsp;"  
		// "&nbsp;&emsp;▲▼▲▼▲&nbsp;&emsp;"  
	}  
public void showHouse(){  
		//作った家を表示するメソッド  
}  

## Q2 大工の抽象クラスを作成し、大工クラスを親とする土台職人、壁職人、屋根職人のクラスを作成せよ。

■抽象クラス:Carpenter  
<フィールド変数>  
名前:name  
<コンストラクタ>  
任意  
＜メソッド＞  
	public abstract void create()  
	
■一般クラス:BaseCraftsman(スーパークラス:Carpenter)  
＜フィールド変数＞  
任意  
<コンストラクタ>  
任意  
＜メソッド＞  
public void create(){  
		//Houseクラスに土台を追加させる。  
		//"this.name+"さんは土台を作った"と表示させる。  
	}   
	
■一般クラス:WallCraftsman(スーパークラス:Carpenter)  
＜フィールド変数＞  
任意  
<コンストラクタ>  
任意  
＜メソッド＞  
public void create(){  
		//Houseクラスに壁を追加させる。  	
		//"this.name+"さんは壁を作った"と表示させる。  
	}   

■一般クラス:RoofCraftsman(スーパークラス:Carpenter)  
＜フィールド変数＞  
任意  
<コンストラクタ>  
任意  
＜メソッド＞  
public void create(){  
		//Houseクラスに屋根を追加させる。  	
		//"this.name+"さんは屋根を作った"と表示させる。  
	}   
	
## Q3Mainメソッドを作り実行例の処理を実現せよ。

[実行例]  
1.家を建てる,2.家を見る,3.終了> 1  
源さんは土台を作った  
北さんは壁を作った  
角さんは屋根を作った  
1.家を建てる,2.家を見る,3.終了> 2  
&nbsp;&nbsp;&nbsp;&emsp;&emsp;▲&nbsp;&nbsp;&nbsp;&emsp;&emsp;   
&emsp;&emsp;▲▼▲&emsp;&emsp;   
&nbsp;&emsp;▲▼▲▼▲&nbsp;&emsp;  
&nbsp;&emsp;|&emsp;&emsp;&emsp;|&nbsp;&emsp;  
&nbsp;&emsp;|&emsp;&emsp;&emsp;|&nbsp;&emsp;  
□□□□□□□  
1.家を建てる,2.家を見る,3.終了>1  
源さんは土台を作った  
北さんは壁を作った  
角さんは屋根を作った  
1.家を建てる,2.家を見る,3.終了>2  
&nbsp;&nbsp;&nbsp;&emsp;&emsp;▲&nbsp;&nbsp;&nbsp;&emsp;&emsp;&nbsp;&nbsp;&nbsp;&emsp;&emsp;▲&nbsp;&nbsp;&nbsp;&emsp;&emsp;   
&emsp;&emsp;▲▼▲&emsp;&emsp;&emsp;&emsp;▲▼▲&emsp;&emsp;   
&nbsp;&emsp;▲▼▲▼▲&nbsp;&emsp;&nbsp;&emsp;▲▼▲▼▲&nbsp;&emsp;  
&nbsp;&emsp;|&emsp;&emsp;&emsp;|&nbsp;&emsp;&nbsp;&nbsp;&emsp;|&emsp;&emsp;&emsp;|&nbsp;&emsp;  
&nbsp;&emsp;|&emsp;&emsp;&emsp;|&nbsp;&emsp;&nbsp;&nbsp;&emsp;|&emsp;&emsp;&emsp;|&nbsp;&emsp;  
□□□□□□□□□□□□□□  
1.家を建てる,2.家を見る,3.終了>1  
源さんは土台を作った  
北さんは壁を作った  
角さんは屋根を作った  
1.家を建てる,2.家を見る,3.終了>1 
源さんは土台を作った  
北さんは壁を作った  
角さんは屋根を作った  
1.家を建てる,2.家を見る,3.終了>1  
源さんは土台を作った  
北さんは壁を作った  
角さんは屋根を作った  
1.家を建てる,2.家を見る,3.終了>2  
&nbsp;&nbsp;&nbsp;&emsp;&emsp;▲&nbsp;&nbsp;&nbsp;&emsp;&emsp;&nbsp;&nbsp;&nbsp;&emsp;&emsp;▲&nbsp;&nbsp;&nbsp;&emsp;&emsp;&nbsp;&nbsp;&nbsp;&emsp;&emsp;▲&nbsp;&nbsp;&nbsp;&emsp;&emsp;&nbsp;&nbsp;&emsp;&emsp;▲&nbsp;&nbsp;&nbsp;&emsp;&emsp;&nbsp;&nbsp;&emsp;&emsp;▲&nbsp;&nbsp;&nbsp;&emsp;&emsp;   
&emsp;&emsp;▲▼▲&emsp;&emsp;&emsp;&emsp;▲▼▲&emsp;&emsp;&emsp;&emsp;▲▼▲&emsp;&emsp;&emsp;&emsp;▲▼▲&emsp;&emsp;&emsp;&emsp;▲▼▲&emsp;&emsp;   
&nbsp;&emsp;▲▼▲▼▲&nbsp;&emsp;&nbsp;&emsp;▲▼▲▼▲&nbsp;&emsp;&nbsp;&emsp;▲▼▲▼▲&nbsp;&emsp;&nbsp;&emsp;▲▼▲▼▲&nbsp;&emsp;&nbsp;&emsp;▲▼▲▼▲&nbsp;&emsp;  
&nbsp;&emsp;|&emsp;&emsp;&emsp;|&nbsp;&emsp;&nbsp;&emsp;|&emsp;&emsp;&emsp;|&nbsp;&emsp;&nbsp;&nbsp;&emsp;|&emsp;&emsp;&emsp;|&nbsp;&emsp;&nbsp;&emsp;|&emsp;&emsp;&emsp;|&nbsp;&emsp;&nbsp;&nbsp;&emsp;|&emsp;&emsp;&emsp;|&nbsp;&emsp;  
&nbsp;&emsp;|&emsp;&emsp;&emsp;|&nbsp;&emsp;&nbsp;&emsp;|&emsp;&emsp;&emsp;|&nbsp;&emsp;&nbsp;&nbsp;&emsp;|&emsp;&emsp;&emsp;|&nbsp;&emsp;&nbsp;&emsp;|&emsp;&emsp;&emsp;|&nbsp;&emsp;&nbsp;&nbsp;&emsp;|&emsp;&emsp;&emsp;|&nbsp;&emsp;  
□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□  
1.家を建てる,2.家を見る,3.終了>1  
もう家を建てる場所がありません  
1.家を建てる,2.家を見る,3.終了>3  
アプリケーションを終了します  
