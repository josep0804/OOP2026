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
/// int i, n=100, sign=1;
/// double sum=0;
/// for(i=0,i<n,i++){
///		sum+=sign*4./(2.*i+1);
/// 	sign*=-1;
/// }
/// System.out.println(sum);
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

### Homework8
```java
public class h8 {
	public static void main(String[] args) {
		int score[][] = new int[5][4];
		for(int i=0; i<5; i++) {
			for(int j=0; j<4; j++) {
				score[i][j] = (int)(Math.random()*101);
			}
		}
		System.out.println("국어\t수학\t사회\t과학\t");
		for(int i=0; i<5; i++) {
			for(int j=0; j<4; j++) {
				System.out.print(score[i][j] + "\t");	
			}
			System.out.println();
		}
	}
}
```
<img width="726" height="621" alt="{EF76420A-2C45-4A01-A24B-3260FC00EA04}" src="https://github.com/user-attachments/assets/086a0143-3924-49e8-a9bd-34b82c8e357c" />

### Homework10
```java
public class h10{
	public static void main(String[] args) { 
			int array_count, max_value, bin_size, display_scale, hist_size;
			if(args.length !=4)
					return;
			array_count = Integer.parseInt(args[0]);
			max_value = Integer.parseInt(args[1]);
			bin_size = Integer.parseInt(args[2]);
			display_scale = Integer.parseInt(args[3]);
			hist_size = max_value/bin_size;
		
			int[] arr = new int[array_count];
			int[] hist = new int[hist_size];
			for (int i=0; i<array_count; i++) {
					arr[i] = (int) (Math.random()*max_value);
			}
			for (int i=0; i<array_count; i++) {
					System.out.print(arr[i] + " ");  
			}
			System.out.println();  
		
			for (int i=0; i<array_count; i++) {
					hist[arr[i]/bin_size]++;
			}
			for (int i=0; i<hist_size; i++) {
					System.out.print(hist[i] + " ");  
			}
			System.out.println();  
		}
}
```
<img width="739" height="615" alt="{93EA3840-FBD8-4F23-9725-8D0929584280}" src="https://github.com/user-attachments/assets/526239e2-30d8-4cc6-a62d-beb469f5f615" />

### Homework11
```java
public class Main {
    public static void main(String[] args) {
        if (args.length != 1) {
            System.out.println("Usage: java StatisticsCalculator <array_count>");
            return;
        }
        
        int array_count = Integer.parseInt(args[0]);
        if (array_count <= 0) {
            System.out.println("Array count must be greater than 0.");
            return;
        }

        int[] arr = new int[array_count];
        for (int i = 0; i < array_count; i++) {
            arr[i] = (int) (Math.random() * 100) + 1; 
        }

        System.out.print("Array elements: ");
        for (int i = 0; i < array_count; i++) {
            System.out.print(arr[i] + " ");  
        }
        System.out.println();

        double sum = 0;
        for (int i = 0; i < array_count; i++) {
            sum += arr[i];
        }
        double arithmeticMean = sum / array_count;
        System.out.printf("Arithmetic Mean: %.4f\n", arithmeticMean);

        double prod = 1.0;
        for (int i = 0; i < array_count; i++) {
            prod *= arr[i];
        }
        double geometricMean = Math.pow(prod, 1.0 / array_count);
        System.out.printf("Geometric Mean: %.4f\n", geometricMean);

        double reciprocalSum = 0;
        for (int i = 0; i < array_count; i++) {
            reciprocalSum += 1.0 / arr[i];
        }
        double harmonicMean = array_count / reciprocalSum;
        System.out.printf("Harmonic Mean: %.4f\n", harmonicMean);

        int[] sortedArr = arr.clone();
        java.util.Arrays.sort(sortedArr);
        
        double median;
        if (array_count % 2 == 1) {
            median = sortedArr[array_count / 2];
        } else {
            median = (sortedArr[array_count / 2 - 1] + sortedArr[array_count / 2]) / 2.0;
        }
        System.out.printf("Median: %.4f\n", median);
    }
}
```
<img width="438" height="260" alt="{5BC0C3AA-8133-495A-A0D4-256EC3587557}" src="https://github.com/user-attachments/assets/ef7e3373-e3ab-4da5-bc47-af21db24cba3" />


### Homework13
```java
import java.util.Scanner;
public class h13 {
	public static void main(String[] args) {
		int out;
		while(true) {
			Scanner scanner = new Scanner(System.in);
			String inputString = scanner.nextLine();
			System.out.println(inputString);
			String[] arrOfStr = inputString.split(" ");
			for (String a : arrOfStr) 
				System.out.println(a);
			if(arrOfStr[1].equals("+")) {
				out = Integer.parseInt(arrOfStr[0])+Integer.parseInt(arrOfStr[2]);
				System.out.print(out);
			}
			else if(arrOfStr[1].equals("-")) {
				
			}
			else if(arrOfStr[1].equals("#")) {
			
			}
			else if(arrOfStr[1].equals("/")) {
			
			}
		
		}
	}
}
```
<img width="739" height="656" alt="{7A2BBD36-11CC-4AD4-8495-BAEA3CE6D382}" src="https://github.com/user-attachments/assets/e33a9048-76ce-4898-bb57-a5ba99e47112" />

### Homework14
```java
class Numbers {
    int num[];
    
    Numbers(int num[]) {
        this.num = num;
    }
    
    double getTotal() {
        double sum = 0;
        for(int i = 0; i < num.length; i++) sum += num[i];
        return sum;
    }
    
    double getArithmaticMean() {
        return getTotal() / num.length;
    }
    
    double getHarmonicMean() {
        double reciprocalSum = 0;
        for(int i = 0; i < num.length; i++) {
            if (num[i] == 0) return 0.0; 
            reciprocalSum += 1.0 / num[i];
        }
        return num.length / reciprocalSum;
    }
    
    double getGeometricMean() {
        double prod = 1.0;
        for(int i = 0; i < num.length; i++) {
            if (num[i] <= 0) return 0.0;
            prod *= num[i];
        }
        return Math.pow(prod, 1.0 / num.length);
    }   
    
    double getMedian() {
        int[] temp = num.clone();
        java.util.Arrays.sort(temp); 
        
        if (temp.length % 2 == 1) {
            return temp[temp.length / 2];
        } else {
            return (temp[temp.length / 2 - 1] + temp[temp.length / 2]) / 2.0;
        }
    }
    
    void sorting() {
        java.util.Arrays.sort(num);
    }
    
    void drawHistogram(int start, int end, int binCount, int scale) {
        int binWidth = (end - start) / binCount;
        int[] bins = new int[binCount];
        
        for (int i = 0; i < num.length; i++) {
            int val = num[i];
            int index = (val - start) / binWidth;
            if (index >= binCount) index = binCount - 1; 
            if (index < 0) index = 0;
            bins[index]++;
        }
        
        System.out.println("--- Histogram ---");
        for (int i = 0; i < binCount; i++) {
            int binStart = start + i * binWidth;
            int binEnd = binStart + binWidth - 1;
            
            System.out.printf("%2d~%2d\t: ", binStart, binEnd);
            
            int symbolCount = bins[i] / scale;
            for (int j = 0; j < symbolCount; j++) {
                System.out.print("#");
            }
            System.out.println(" (" + bins[i] + ")");
        }
    }
    
    void display() {
        System.out.printf("%3d : ", num.length);      
        for(int i = 0; i < num.length; i++) 
            System.out.printf("%3d ", num[i]);
        System.out.println();
    }   
}

public class Main {
    public static void main(String[] args) {
        int size = 100;
        int data[] = new int[size];
        for(int i = 0; i < size; i++) 
            data[i] = (int)(Math.random() * 100);
            
        Numbers obj = new Numbers(data);
        obj.display();
        
        System.out.printf("Arithmetic Mean : %5.2f\n", obj.getArithmaticMean());
        System.out.printf("Geometric Mean  : %5.2f\n", obj.getGeometricMean());      
        System.out.printf("Harmonic Mean   : %5.2f\n", obj.getHarmonicMean());      
        System.out.printf("Median          : %5.2f\n", obj.getMedian());      
        System.out.println();
        
        obj.drawHistogram(0, 100, 10, 1);
    }
}
```
<img width="732" height="432" alt="{40ACA7CD-0150-4966-8837-F872F9C4433F}" src="https://github.com/user-attachments/assets/0b09079d-529d-48db-bf90-96da961dce95" />



