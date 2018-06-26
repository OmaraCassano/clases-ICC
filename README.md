# clases-ICC
import os
import sys

n = [10,1,2,6,5,8,]
#1. comparar por parte
def bubble_sort(a):
    for j in range(len(a)):
        for i in range(len(a)-1):
             if a[i]>a[i+1]:
                 #cambiamos
                 temp = a[i]
                 a[i]=a[i+1]
                 a[i+1]=temp
        #print(j, a)
    return a

#print(bubble_sort(n))

def select_sort(lista):
    for i in range(len(lista)):
        min = i
        for j in range (i, len(lista)):
            if lista[j]<lista[min]:
                min = j
            temp = lista[i]
            lista[i] = lista [min]
            lista[min] = temp
        return lista

print(select_sort(n))
viene desde tuplas, diccionarios y esta clse de metodos de ordenamiento y si o si viene ordenamiento de tuplas
