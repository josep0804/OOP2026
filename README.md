# OOP2026
### Homework1
```java
public class Homework1{
  public static void main(String []args){
    int i, j;
    for(i=0; i<10; i++) {
      for(j=0; j<10; j++) {
        System.out.print("#");
      }
      System.out.println("");
    }
  }
}
```
<img width="1000" height="744" alt="{AA2C7E43-FDBD-4EBB-8B95-6DE9F54C2F37}" src="https://github.com/user-attachments/assets/65275305-6c0f-4722-99c1-4d1db28f6ef6" />

### Homework2
```java
public class aw {
	public static void main(String[] args) {
		int a = 1, b = 1, c;
		System.out.print("1 1 ");
		int i;
		for(i=0; i<20; i++) {
		  c = a + b;
		  System.out.print(c+" ");
		  a = b;
		  b = c;
		}
	}
}
```
<img width="710" height="399" alt="{F78933C7-C329-4518-B3D7-804ECF201078}" src="https://github.com/user-attachments/assets/a5ff9531-ec7b-4bfb-aa7e-ceb110eadf4d" />

### Homework3
```java
public class c3 {
	public static void main(String[] args) {
		int a = 1;
		int b = 2;
		for(int i=0; i<20; i++){
			int c = a+b;
			a = b;
			b = c;
			System.out.println(b+"/"+a+"="+(double)b/a);
		}
	}
}
```
<img width="739" height="664" alt="{B8668900-F511-455F-B76E-5671F3861BED}" src="https://github.com/user-attachments/assets/e47f293d-33ca-42f3-9e5c-5599646a3f0a" />

### Homework4
```java
public class h4 {
	public static void main(String[] args) {
		for(int i =1; i<10; i+=1) {
			for(int j=1; j<10; j++) { 
				System.out.print(j+"*"+i+"="+(i*j)+"\t");
			}
			System.out.println();
		}
	}
}
```
<img width="733" height="504" alt="{DA70D68E-E13F-4B66-86C7-A16E116336DB}" src="https://github.com/user-attachments/assets/35a1b9c5-3de2-4ba7-821d-afacf190f556" />

### Homework5
```java
public class h5 {
	public static void main(String[] args) {
		double pi = 0;
		for (int i = 0; i<100; i++) {
			pi += Math.pow(-1, i) / ((2 * i +1) * Math.pow(3, i));
		}
		pi = Math.sqrt(12) * pi;
		System.out.println(pi);
	}
}
```
<img width="719" height="392" alt="{CCB5CBC9-EE59-4092-B01F-6E4F7A9BE72E}" src="https://github.com/user-attachments/assets/4b62d470-1d89-4dd2-a902-4b4807ad7eba" />

### Homework6
```java
public class h6 {
	public static void main(String[] args) {
		int binomial[][] = new int[10][10];
		for (int i = 0; i<10; i++) {
			binomial[i][0] = 1;
			binomial[i][1] = 1;
			
			for(int j = 1; j<i; j++) {
				binomial[i][j] = binomial[i-1][j-1] + binomial[i-1][j];
			}
		}
		for(int i = 0; i<10; i++) {
			for(int j = 0; j<=i;j++) {
				System.out.print(binomial[i][j] + "\t");
			}
			System.out.println();
		}
	}
}
```
<img width="738" height="589" alt="{90E4B1E3-C9FD-4654-BD24-3D51370616A8}" src="https://github.com/user-attachments/assets/d8a97833-3a3a-4fd3-8c00-c861221fc371" />

### Homework7
```java

public class h7 {
	public static void main(String[] args) {
		int data[] = new int[20];
		for(int i=0; i<20; i++)
		    data[i]=(int)(Math.random()*100);
		for(int i=0; i<20; i++)
		    System.out.println(data[i]);
	}
}

```
<img width="738" height="560" alt="{EE72AB31-704E-4AC7-8140-FE27A67B7959}" src="https://github.com/user-attachments/assets/a537f4e6-0659-42b2-a335-0259f3ad35c1" />

