#include<iostream>
using namespace std;
class complex{
	int real,img;
	public:
		complex(){
			real=2;
			img=4;
		}
		complex(int r,int i){
			real=r;
			img=i;
		}
		void addcomplex(complex c1,complex c2){
			real=c1.real+c2.real;
			img=c1.img+c2.img;
		}
		void display(){
			cout<<real<<"+"<<img<<"i"<<endl;
		}
};
int main(){
	complex c1;
	complex c2(10,20);
	complex c3;
	cout<<"first complex number=";
	c1.display();
	cout<<"second complex number=";
	c2.display();
	c3.addcomplex(c1,c2);
	cout<<"first complex number=";
	c3.display();
	return 0;
}
