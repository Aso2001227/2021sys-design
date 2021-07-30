public class Game { Ship ship1 = new Ship(); Ship ship2 = new Ship(); Ship ship3 = new Ship();

public void display(){ Scanner sc = new Scanner(System.in);
int turn = 1;int i = 1;
while(Ship.finish()!=true){ 
System.out.println("ターン"+turn+"); 
if(ship1.shipdie() == false){
System.out.println("船1：生きてる"); 
}else{ System.out.println("船1：撃沈"); 
}
if(ship2.shipdie() == false){
System.out.println("船2：生きてる");
}else{ System.out.println("船2：撃沈"); 
}
if(ship3.shipdie() == false){
System.out.println("船3：生きてる"); 
}else{ System.out.println("船3：撃沈");
}
