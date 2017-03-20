# The test program of mini-vm interpreter

The program get a text string from a user, and print a simple cipher text. In a cipher process, each value of the input text is decreased by 2. 

# Example
- input : abcdefghijklmnopqrstuvwxyz
- output: _`abcdefghijklmnopqrstuvwx

- input : [IS521]Hello,I_finished_HW.
- output: YGQ30/[Fcjjm*G]dglgqfcb]FU,

# Pseudocode
int main(){
	char* buf = malloc(/* some amount */);
	printf("Text: ");
	gets(buf);

	int cnt = 0;
	while(*(buf+cnt) != '\0'){
		*(buf+cnt) -= 2;
		cnt++;
	}

	printf("Cipher Text: %s", buf);

	return 0;
}