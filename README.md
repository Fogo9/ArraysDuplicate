# **ARRAYS DUPLICATE**

## INFORMATION

* **Program to find repeating even numbers in arrays.**

## TECHNOLOGIES USED

* **JAVA**

## CONTENTS

* The variables **int** and **boolean** are defined.

* It checks whether it is true or false with a boolean variable.

* Sorts numbers in arrays from smallest to largest with the definition of sort.

* Identify and print even even numbers with a for loop.

## CODES

```Java

        import java.util.Arrays;

        public class ArraysDuplicate{

            static boolean isFind(int[] arr, int value){

                for(int i : arr){

                    if(i == value){

                        return true;

                    }
                }

                return false;

            }


```

```Java

            public static void main(String[] args){

                int[] list = {4, 6, 9, 11, 14, 4, 8, 6, 2, 2, 14,8};

                Arrays.sort(list);

                int[] duplicate = new int[list.length];

                int startIndex = 0;

                for(int i = 0; i < list.length; i++){

                    for(int j = 0; j < list.length; j++){

                        if((i != j) && (list[i] == list[j])){

                            if(!isFind(duplicate, list[i])){

                                duplicate[startIndex++] = list[i];

                            }

                            break;

                        }
                    }
                }

                for(int value : duplicate){

                    if(value != 0 && value % 2 == 0){

                        System.out.println(value);

                    }
                }
            }
        }

```

```bash

    2
    4
    6
    8
    14

```

<br />

## LINK

* Click here https://github.com/Fogo9/ArraysDuplicate.git to access the Github page for this project.

<br />

## LICENSE

* This software is licensed By Tuncay Demir under the MIT license.

<br />

>[Patika.dev](https://app.patika.dev/fogomurphy)

<br/>

| Name |  Email |
| ---- |  ----- |
| Tuncay | tuncaydemir682@gmail.com |
