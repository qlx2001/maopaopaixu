# maopaopaixu
冒泡排序原理代码
public class Example01 {
	public static void main(String[] args) {
		int[] arr={9,8,3,5,2};
		for (int i=0;i<arr.length;i++){
			System.out.print(arr[i]+" ");
		}
		System.out.println();			
		for(int i=1;i<arr.length;i++){
			for(int j=0;j<arr.length-i;j++){
				if(arr[j]>arr[j+1]){	
					int temp=arr[j];
					arr[j]=arr[j+1];
					arr[j+1]=temp;
				}
			}
		}
		for(int i=0;i<arr.length;i++){
			System.out.print(arr[i]+" ");
		}
	}
}


import static org.junit.jupiter.api.Assertion.*;
class Example01Test {
private static int normalSort[] = {9,8,3,5,2};
@BeforeEach
viod setUp() throws Exception {
}
@Test 
void testBSort () {
int a[] = {9,8,3,5,2};
Example01.BSort(a);
assertArrayEqual s(normalSort, a);
}
}
