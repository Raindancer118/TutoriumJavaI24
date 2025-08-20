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
public class Tamagotchi{
    // Status:
    private int hunger = 0;
    private int mood = 0;
    private int fatigue = 0;
    
    // Schwellwerte:
    private int hungerThresold;
    private int moodThresold;
    private int fatigueThresold;
    
    public Tamagotchi(int hT, int mT, int fT) {
        hungerThresold = hT;
        moodThresold =mT;
        fatigueThresold = fT;
    }
    
    public void play() {
        if (isHungry()) return;
        else {
            hunger = hunger + 2;
            mood = mood +2;
            fatigue = fatigue +3;
        }        
    }
    
    public void eat(){
        if (isTired()) return;
        else {
            hunger = hunger -3;
            fatigue = fatigue +2;
        }
    }
    
    public void sleep(){
        if (isHungry()) {
            hunger++;
            mood--;
        }
        else {
            hunger++;
            mood++;
        }
        fatigue = 0;
    }
    
    public void pet(){
        hunger++;
        mood = mood +2;
    }
    
    private boolean isHungry(){
        if (hunger > hungerThresold) return true;
        else return false;
    }
    
    private boolean isTired(){
        if (fatigue > fatigueThresold) return true;
        else return false;
    }
    
    private boolean isHappy(){
        if (mood > moodThresold) return true;
        else return false;
    }
    
    public String getGeneralCondition(){
        if (isTired()) return "tired";
        if (isHungry()) return "hungry";
        if (isHappy()) return "happy";
        else return "indifferent";
    }
    
    public void makeHappy(){
        eat();
        play();
        sleep();
    }
}
```