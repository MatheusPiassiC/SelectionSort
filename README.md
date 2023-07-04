# SelectionSort(C++)
Teste do método de ordenação Selection Sort, ordenando um vetor em ordem crescente;
#include <iostream>


#include <iostream>

using namespace std;

void ordena(int vetor[], int tamanho){
	int i, j, menor, troca;
	for(i=0; i<tamanho; i++){
		menor=i;
		for(j=i+1; j<tamanho; j++){
			if(vetor[j]<vetor[menor]){
				menor=j;
				}
			}
		troca=vetor[i];
		vetor[i]=vetor[menor];
		vetor[menor]=troca;
		}
	}

int main(){
	int tam=5, i;
	int vetor[tam]={12,4,7,9,3};
	ordena(vetor, tam);
	for(i=0; i<tam; i++){
		cout<<vetor[i]<<" ";
		}
	return 0;
	}
