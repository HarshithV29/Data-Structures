INSERTION SORT
def insertionsort(arr,n):
  for i in range(1,n):
    temp=arr[i]
    j=i-1
    while j>=0 and temp<arr[j]:
      arr[j+1]=arr[j]
      j-=1
      arr[j+1]=temp
  return arr
arr=[4,5,7,2,6,3]
n=len(arr)
result=insertionsort(arr,n)
print("the sorted array is: ", result) 


OUTPUT:-
the sorted array is:  [2, 3, 4, 5, 6, 7]
