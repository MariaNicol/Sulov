# Sulov
------------
int n, p , k; 
    cin>>n; 
    cin>>p ; 
while ((n!=0)&&(k!=p))
    { 
    k=n%10;
    n/=10;}
     if ( k==p) cout<<"yes"<<k<<" "<<p;
    else cout<<"no";
    return 0;
    --
    int n,k, sum=0; 
    cin>>n;
    while ( n!=0) 
    {
       k= n%10;
       sum= sum+k;
       n=n /10;

    }
cout<<"sum = "<<sum;
    return 0;


---------------------
 
08.06.2025 
//1. намира макс нечетно от 3 
 if (a % 2 != 0) max = a;
    else if (b % 2 != 0) max = b;
    else if (c % 2 != 0) max = c;
    else {
        cout << "Няма нечетни числа";
        return 0;
    }

    if (b % 2 != 0 && b > max) max = b;
    if (c % 2 != 0 && c > max) max = c;

  cout<<max;
---------- 2 
int main() 
{
    int g; 
    cin >> g;
    cout << ((g % 4 == 0 && g % 100 != 0) || (g % 400 == 0) ? "yes" : "no");
    return 0;
}

--- 3
int a, min, max;
cin>>a;
min=a; 
max=a;
while(a!=0) {
  if ( max<=a) { max = a; }
  if ( min>=a) min=a; 
  cin>>a;
}
cout<<min<<" "<<max;
------------- 4
int n; 
cin>>n;
 while ((n<5)||(n>50)) {

  cout<<"nekorekton vhod"<<endl;  
  cin>>n;
}

cout<<n*n;

-------- 5 
int n,p ;
cin>>n;
for ( int i=0; i<n; n++)
{ p=n%10; 

}
cout<<p;
----------
int n,m; 
cin>>n>>m; 

for ( int i =n; i<m; i++)
 { 
   if (i%5==0) cout<<i<<endl; 

 } 
    return 0;
}



 ---------------------------- З А Д А Ч И  Н А  С / С + + ----------------------------
   int a, b, c;
	   complex<double> x1, x2;
	   double D;
	   cin >> a >> b >> c;
	   D = b * b - 4 * a * c;
	   if (D > 0) {
		   x1 = (-b + sqrt(D)) / (2.0 * a);
		   x2 = (-b - sqrt(D)) / (2.0 * a);
		   cout << "Realni koreni: " << x1 << " i " << x2 << endl;
	   }
	   else if (D == 0) {
		   x1 = x2 = -b / (2.0 * a);
		   cout << "D=0, edin koren: " << x1 << endl;
	   }
	   else {
		   x1 = complex<double>(-b / (2.0 * a), sqrt(-D) / (2.0 * a));
		   x2 = complex<double>(-b / (2.0 * a), -sqrt(-D) / (2.0 * a));
		   cout << "Kompleksni koreni: " << x1 << " i " << x2 << endl;
	   }
	   return 0;  */
	   // таблица за умножение 
	  /* int n, t; cin >> n;
	   for (int i = 0; i <= 10; i++)
	   {
		   t = i * n;
		   cout << t << endl; }*/
		/*int n;
		cin >> n; 
		if (n < 0) cout << "Only positive numbers" << endl;
		  else  if (n % 2 == 0) cout << "4etnite nums ne sa prosti" << endl;
			else if (n == 1 || n == 0) cout << " Edno i nula ne sa prosto nums" << endl;
			  else */ 
		// obratno cislo 
		/*int n, rn = 0;
		cin >> n;
		while (n)
		{	rn = n % 10 + rn * 10;
			n= n / 10;
		}   cout << rn;
		*/  
		///
		int n,v,sum=0;
		cout << "br nums"<<endl;
		cin >>  n;
		cout << "the numbers: " << endl;
		cin >> v;
		//for (int i = 0; i <= n; i++)
				for (int j = 0; j <= n; j++)
			{	sum = sum + j;	}
		cout << sum<<endl;
	}
----------------------------------------------------------------------> 							<--------------------------------------------------------------------------------
		// sum till num 
	/*int n, sum = 0;
	cin >> n;
	for (int i = 0; i <= n; i++)
	{
		sum = sum + i; 
	}
	cout << sum;*/
	//факториел
	/*int n, f = 1;
	cin >> n;
	for (int i = 1; i <= n; i++)
	{
		f = f * i;
	}
	cout << f; */
	------------------
	напавете : 1. въведете n бр числа 2. намерете Сума на въведени от нас числа 
		int num,n,sum=0; 
		cout << "input br nums " << endl;
		cin >> n;
		cout << "the nums"<<endl;
		for(int i=0;i<n;i++)
		{		
			cin >> num;
			sum=sum+ num;
		}
		cout <<"sum: "<< sum;
	------------
	average&sum of n nums:
	int n, num,average=0,sum=0;
		cin >> n;
	   for (int i=0; i<n;i++)
	   {
		   cin >> num;
		   sum += num;
		   average =  sum/n;
	   }
	   cout << "Sum: " << sum << " ,Agerage: " << average;
	   --------------------
	   извежда таблицата за умножение на въведено от нас число
	   int n,p=1; 
		cin >> n;
		for (int i = 1; i <= 10; i++)
		{
			p = i * n;cout << p<<endl;
		}
	   ---------------------
	   намира сума на нечетни числа , въведени от нас 
	   int n,num, sum = 0; 
		cin >> n;
		for(int i=0; i<n; i++)
		{
			cin >> num;
			if (num % 2 == 1) sum += num;		
		}cout <<"Sum na ne4etnite (vuvedeni) 4isla = " << sum;
		----------------------------------------------------------------------------//////////////////////////////////////////////////////////////////////////////////////////////////		
	04.03	int x, k;
		cin >> x;
		k = x * 5+2-14%x;
		cout << k;
		--------------
		int qty;
		double  price , dds, cbd; //cbd = cena s dds	
		cout << "enter qty: "<<endl; cin >> qty;
		cout << "enter price: "<<endl; cin >> price;
		cbd = qty * price; cout << "Cena bez DDS= " << cbd << endl; // ok
     	dds = (cbd*1.2)-cbd;  cout << "Stoinost na DDS= " << dds << endl;
		// 2РО РЕШЕНИЕ ЗА ? ДДС--> УМНОЖАВАМЕ ПО 0,2 И НАМИРАМЕ ДИРЕКНО ДДС, АКО * 1,2О ТРЯБВА ДА СЕ ВАДИ НАЧАЛНТА СТОЙНОСТ 
		cout << "Kraina cena= " << cbd + dds << endl;
		-----------
		int n, a, b, c;
		cin >> n;
		a = n / 100; cout << a<<endl;
		b = n % 100/10; cout << b<<endl;
		c = n % 10; cout << c << endl;
		-------------
			double PI = 3.14, r, S, P; cin >> r;
		S =  r * r*PI;
		P = 2 * PI * r; cout << "s= " << S << "P= " << P << endl;
		-------------  05.03.2025
		int n; 
		cin >> n; 
		for (int i = 1; i <= n; i++)
		{
			for (int j = 1; j <= i; j++)
			{
				cout << j;
			} cout << endl;
		}// изход ако n=5
			//1
			//12
			//123
			//1234
			//12345
		-------------
		!! различна е от горнат!!!
		int n; cin >> n;
		for (int i=1; i<=n; i++)
		{
			for (int j = 1; j<=i; j++)
			{
				cout << i;
			}
			cout << endl;
		}
		-------------
	10.03	int n, i, j, k = 1; 
		cin >> n; 
		for( i=1; i<=n; i++)
		{
			for (j = 1; j <= n - i; j++)
			{
				cout << " ";
			}		
			for (j = 1; j <= i; j++)
			{
				cout <<i <<" ";
			} cout << endl;
		}
		--------------------
		setlocale(LC_ALL, "Bulgarian");
		int ah, a, AH, A; 
		cin >> ah >> a >> AH >> A;
		int s = (a * ah)/2; 
		int S = (A * AH) / 2; 
		if (S > s) cout << "По- голямото лице е S= " << S;
		else cout << "По- голямото лице е s= " << s;
		------------------------
		17.03 
		double a, b, c,max; 
		cout << "Въведи числата ";
		cin >> a >> b >> c;
		max = a;
		if (b > max) max = b;  // !!!!!!!!!!!!!!!!!!!!!!!!!!!! П Р О В Е Р Я В А Н Е  С  М А Х !!!!!! НЕ С a !!!! 
		if (c > max) max = c;
		cout << "Max is " << c;
		----------------------
		int x,y,z,a;
		cout << " Въвеждане на числата: ";
		cin >> x >> y >> z;
		if (x>y)
		{
			a = x;
			x = y;
			y = a;
		}
		if (y > z)
		{
			a = y;
			y = z;
			z = a;
		}
		if (x > z)
		{
			a = x;
			x = z;
			z = a; 
		}
		cout << x << " " << y << " " << " " << z; !!!!!!!!!!!!!!!!!!!!!!!!
-------------
int age; 
		cout << "Въведи години на клиента: "; cin >> age;
		if (age >= 1 && age < 18) cout << "Не може да влезе в киното";
		else cout << "Може";
------------
double km, cena; 
		cin >> km; 
		if (km <= 3.0) { cena = km * 1.50; cout <<cena ; }
		if (km > 3.0) { cena = 1.50 * 3 + (km-3) * 1.20; cout << cena; }
		------ 21.03.2025 ---
		double a, b, c, max, br = 0;
	cin >> a >> b >> c;
	if (a == b && b== c) cout << "и трите са еднакви" << endl;
	if (a == b || a == c || c == b) cout << "има две ендакви" << endl;
	else { cout << "Nqma" << endl; }
	max = a;
	if (b >= max) max = b;
	if (c >= max) max = c;
	cout << "Max is:" << max;
	----------------
	int a, b, c,max;
	cin >> a >> b >> c;
	max = a;
	if (b >= max && b % 2 == 1)
	{
		 max=b;
	}
	if (c >= max && c % 2 == 1)
	{
		 max=c;
	}
	cout << max;
	----------------------------
	26.05
	#include <iostream>
#include <limits>

using namespace std;
int main()
{

int arr[10], br1=0;
int br2=0,i;
int *p=arr; 

for (  i=0; i<10; i++)
{ 
cin>>*p; p++; 
}

for ( i=9; i>=0; i--)
{ p--; 
cout<<*p;}

for( i=0; i<10; i++){
if(*p%2==0) 
{br1++;} //br четни 
else {br2++;} // нечетни 
p++;
} 
if ( br1>br2) cout<<1;
if ( br1<br2) cout<<2;
if ( br1==br2) cout<<0; ///!!!
}
