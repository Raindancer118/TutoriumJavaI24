# Test zu Foliensatz 2
## Frage 1
![[Test zu Foliensatz 2- Frage 1.png]]
## Frage 2
![[Test zu Foliensatz 2- Frage 2.png]]
## Frage 3
![[Test zu Foliensatz 2- Frage 3.png]]
## Frage 4
```
public class Module {
    private String code;
    private String name;
    private int contactHours;
    
    public Module(String _code, String _name){
        code=_code;
        name=_name;
    }
    public void setName(String _name){
        name=_name;
    }
    public String getName(){
        return name;
    }
    public String getCode(){
        return code;
    }
    public void setContactHours(int hours){
        contactHours = hours;
    }
    public int getContactHours(){
        return contactHours;
    }
}
```
## Frage 5
![[Test zu Foliensatz 2- Frage 5.png]]
## Frage 6
![[Test zu Foliensatz 2- Frage 6.png]]
## Frage 7
```
//Vervollständigen Sie folgende Methode
public int relativeXPositionTo(Point p) {
    if (this.x == p.x) return 0;
    if (this.x > p.x) return 1;
    return -1;
}
```
## Frage 8
```
public class Tamagotchi {  
    // Exemplarvariablen  
    //Status    private int hunger = 0;  
    private int mood = 0;  
    private int fatigue = 0;  
    //Schwellwerte  
    private int hungerTreshold;  
    private int fatigueTreshold;  
    private int moodTreshold;  
  
    // Konstruktor  
    public Tamagotchi(int hungerTreshold, int fatigueTreshold, int moodTreshold) {  
        this.hungerTreshold = hungerTreshold;  
        this.fatigueTreshold = fatigueTreshold;  
        this.moodTreshold = moodTreshold;  
    }  
  
    // Methoden  
    public void play() {  
        if(!isHungry()) {  
            hunger += 2;  
            mood += 2;  
            fatigue += 3;  
        }  
    }  
  
    public void sleep() {  
        if(isHungry()) {  
            hunger++;  
            mood--;  
            fatigue = 0;  
        }  
        else {  
            hunger++;  
            mood++;  
            fatigue = 0;  
        }  
    }  
  
    public void eat() {  
        if (!isTired()) {  
            hunger -= 3;  
            fatigue += 2;  
        }  
    }  
  
    public void pet() {  
        hunger++;  
        mood += 2;  
    }  
  
    public String getGeneralCondition() {  
        if (isTired()) return "tired";  
        if (isHungry()) return "hungry";  
        if (isHappy()) return "happy";  
        return "indifferent";  
    }  
  
    public void makeHappy() {  
        eat();  
        play();  
        sleep();  
    }  
  
    // Helper  
    private boolean isHungry() {  
        return (hunger > hungerTreshold);  
    }  
  
    private boolean isTired() {  
        return (fatigue > fatigueTreshold);  
    }  
  
    private boolean isHappy(){  
        return (mood > moodTreshold);  
    }  
}
```