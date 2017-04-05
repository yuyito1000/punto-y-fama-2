# punto-y-fama-2#include <iostream>
#include <cstdlib>
#include <cmath>
#include <iomanip>
#include <sstream>
#include <time.h>
#include <conio.h>

using namespace std;

int main()
{
	int k1 = 0, k2 = 0, k3 = 0, k4 = 0, m, n, o, p, contador = 0, control = 0, k;

	srand(time(NULL));

	cout << "Puntos y Famas !!!" << endl;
    
	cout << "INSTRUCCIONES: \n" << endl;

	while (k1 == k2 || k1 == k3 || k1 == k4 || k2 == k3 || k2 == k4 || k3 == k4)
	{
		k1 = rand() % 10;
		k2 = rand() % 10;
		k3 = rand() % 10;
		k4 = rand() % 10;
	}

	cout << "El numero aleatorio generado es: " << k1 << "" << k2 << "" << k3 << "" << k4 << endl;

	do 
	{
		cout << "Ingrese un numero de 4 digitos \n";
		cin >> k;
		
		n = (k / 1000);
		m = (k - (n * 1000)) / 100;
		o = (k - ((n * 1000) + (m * 100))) / 10;
		p = (k - ((n * 1000) + (m * 100) + (o * 10)));

		cout << n << "" << m << "" << o << "" << p << "" << endl;

		if (n == k2 || n == k3 || n == k4)
		{
			if (m == k1 || m == k3 || m == k4)
			{
				if (o == k1 || o == k2 || o == k4)
				{
					if (p == k1 || p == k2 || p == k3)
					{
						cout << "Puntos: \t P P P P \n Famas: " << endl;
					}
					else
					{
						if (p == k4)
						{
							cout << "Puntos: \t P P P \n Famas: \t F " << endl;
						}
						else
						{
							cout << "Puntos: \t P P P \n Famas: " << endl;
						}
					}
				}
				else
				{
					if (o==k3)
					{
						if (p == k1 || p == k2)
						{
							cout << "Puntos: \t P P P \n Famas: \t F " << endl;
						}
						else
						{
							if (p == k4)
							{
								cout << "Puntos: \t P P \n Famas: \t F F " << endl;
						    }
							else
							{
								cout << "Puntos: \t P P \n Famas: \t F " << endl;
							}
						}
				    }
					else
					{
						if (p == k1 || p == k2 || p == k3)
						{
							cout << "Puntos \t P P P \n Famas:  " << endl;

					    }
						else
						{
							if (p==k4)
							{
								cout << "Puntos: \t P P \n Famas: \t F " << endl;
							}
							else
							{
								cout << "Puntos: \t P P \n Famas: \t F " << endl;
							}
						}
					}
				}
			}
			else
			{
				if (m == k2)
				{
					if (o == k1 || o == k4)
					{
						if (p == k1 || p == k3)
						{
							cout << "Puntos: \t P P P \n Famas: \t F"<<endl;
						}
						else
						{
							if (p == k4)
							{
								cout << "Puntos: \t P P \n Famas: \t F F " << endl;
							}
							else
							{
								cout << "Puntos: \t P P \n Famas: \t F " << endl;
							}
						}
					}
					else
					{
						if (o == k3)
						{
							if (p == k1)
							{
								cout << "Puntos: \t P P \n Famas: \t F F " << endl;
							}
							else
							{
								if (p == k4)
								{
									cout << "Puntos: \t P \n Famas: \t F F F " << endl;
								}
								else
								{
									cout << "Puntos: \t P \n Famas: \t F F " << endl;
								}
							}
						}
						else
						{
							if (p == k1 || p == k3)
							{
								cout << "Puntos: \t P P \n Famas: \t F " << endl;
							}
							else
							{
								if (p == k4)
								{
									cout << "Puntos: \t P \n Famas: \t F F " << endl;
								}
								else
								{
									cout << "Puntos: \t P \n Famas: \t F " << endl;
								}
							}
						}
					}
				}
				else
				{
					if (o == k1||o==k4||o==k2)
					{
						if (p == k1 || p == k3 || p == k2)
						{
							cout << "Puntos: \t P P P \n Famas: \t " << endl;
						}
						else
						{
							if (p == k4)
							{
								cout << "Puntos: \t P P \n Famas: \t F " << endl;
							}
							else
							{
								cout << "Puntos: \t P P \n Famas: \t " << endl;
							}
						}
					}
					else
					{
						if (o == k3)
						{
							if (p == k1 || p == k3 || p == k2)
							{
								cout << "Puntos: \t P P \n Famas: \t F " << endl;
							}
							else
							{
								if (p == k4)
								{
									cout << "Puntos: \t P \n Famas: \t F F " << endl;
								}
								else
								{
									cout << "Puntos: \t P \n Famas: \t F " << endl;
								}
							}
						}
						else
						{
							if (p == k1 || p == k3 || p == k2)
							{
								cout << "Puntos: \t P P \n Famas: \t " << endl;
							}
							else
							{
								if (p == k4)
								{
									cout << "Puntos: \t P \n Famas: \t F " << endl;
								}
								else
								{
									cout << "Puntos: \t P \n Famas: \t  " << endl;
								}
							}
						}
					}
				}
			}
		}
		else
		{
			if (n == k1)
			{
				if (m == k3 || m == k4)
				{
					if (o == k2 || o == k4)
					{
						if (p == k2 || p == k3)
						{
							cout << "Puntos: \t P P P \n Famas: \t F " << endl;
						}
						else
						{
							if (p == k4)
							{
								cout << "Puntos: \t P P \n Famas: \t F F " << endl;
							}
							else
							{
								cout << "Puntos: \t P \n Famas: \t F F " << endl;
							}
						}
					}
					else
					{
						if (o == k3)
						{
							if (p == k2)
							{
								cout << "Puntos: \t P P \n Famas: \t F F " << endl;
							}
							else
							{
								if (p == k4)
								{
									cout << "Puntos: \t P \n Famas: \t F F F " << endl;
								}
								else
								{
									cout << "Puntos: \t P \n Famas: \t F F " << endl;
								}
							}
						}
						else
						{
							if (p == k2)
							{
								cout << "Puntos: \t P P \n Famas: \t F " << endl;
							}
							else
							{
								if (p == k4)
								{
									cout << "Puntos: \t P \n Famas: \t F F " << endl;
								}
								else
								{
									cout << "Puntos: \t P \n Famas: \t F " << endl;
								}
							}
						}
					}
				}
				else
				{
					if (m == k2)
					{
						if (o == k4)
						{
							if (p == k3)
							{
								cout << "Puntos: \t P P \n Famas: \t F F " << endl;
							}
							else
							{
								if (p == k4)
								{
									cout << "Puntos: \t P \n Famas: \t F F F " << endl;
								}
								else
								{
									cout << "Puntos: \t P \n Famas: \t F F " << endl;
								}
							}
						}
						else
						{
							if (o == k3)
							{
								if (p == k4)
								{
									cout << "Puntos: \t \n Famas: \t F F F F" << endl;
								}
								else
								{
									cout << "Puntos:\t \n Famas: \t F F F " << endl;
								}
							}
							else
							{
								if (p == k3)
								{
									cout << "Puntos: \t P \n Famas: \t F F " << endl;
								}
								else
								{
									if (p == k4)
									{
										cout << "Puntos: \t \n Famas: \t F F F " << endl;
									}
									else
									{
										cout << "Puntos: \t \n Famas: \t F F " << endl;
									}
								}
							}
						}
					}
					else
					{
						if (o == k2 || o == k4)
						{
							if (p == k2 || p == k3)
							{
								cout << "Puntos: \t P P \n Famas: \t F " << endl;
							}
							else
							{
								if (p == k4)
								{
									cout << "Puntos: \t P \n Famas: \t  F F " << endl;
								}
								else
								{
									cout << "Puntos: \t P \n Famas: \t F " << endl;
								}
							}
						}
						else
						{
							if (o == k3)
							{
								if (p == k2)
								{
									cout << "Puntos: \t p \n Famas: \t F F " << endl;
								}
								else
								{
									if (p == k4)
									{
										cout << "Puntos: \t \n Famas: \t F F " << endl;
									}
									else
									{
										cout << "Puntos: \t \n Famas: \t F F " << endl;
									}
								}
							}
							else
								if (p == k3 || p == k2)
								{
									cout << "Puntos: \t P \n Famas: \t F " << endl;
								}
								else
								{
									if (p == k4)
									{
										cout << "Puntos: \t Famas: \t F F " << endl;
									}
									else
									{
										cout << "Puntos: \t Famas: \t F " << endl;
									}
								}
						}
					}
				}
			}
		}
		else
		{
			if (m == k1 || m == k3 || m == k4)
			{
				if (o == k1 || o == k2 || o == k4)
				{
					if (p == k1 || p == k2 || p == k3)
					{
						cout << "Puntos: \t P P \n Famas: \t F " << endl;
					}
					else
					{
						cout << "Puntos: \t P P \n Famas: \t " << endl;
					}
				}
			}
			else
			{
				if (o == k3)
				{
					if (p == k1 || p == k2)
					{
						cout << "Puntos: \t P \n Famas: \t F " << endl;
					}
					else
					{
						if (p == k4)
						{
							cout << "Puntos: \t P \n Famas: \t F F " << endl;
						}
						else
						{
							cout << "Puntos: \t P \n Famas: \t F " << endl;
						}
						
					}
				}
				else
				{
					if (p == k1 || p == k2 || p == k3)
					{
						cout << "Puntos: \t P P \n Famas: \t" << endl;
					}
					else
					{
						if (p == k4)
						{
							cout << "Puntos: \t P \n Famas: \t F " << endl;
						}
						else
						{
							cout << "Puntos: \t P \n Famas: \t " << endl;
						}
					}
				}
			}

		}
		else
		{
			if (m == k2)
			{
				if (o == k1 || o == k4)
				{
					if (p == k1 || p == k3)
					{
						cout << "Puntos: \t P P \n Famas: \t F " << endl;
					}
					else
					{
						if (p == k4)
						{
							cout << "Puntos: \t P \n Famas: \t F F " << endl;
						}
						else
						{
							cout << "Puntos: \t P \n Famas: \t F " << endl;
						}
					}
				}
				else
				{
					if (o == k3)
					{
						if (p == k1)
						{
							cout << "Puntos: \t P \n Famas: \t F F " << endl;
						}
						else
						{
							if (p == k4)
							{
								cout << "Puntos: \t \n Famas: \t F F F " << endl;
							}
							else
							{
								cout << "Puntos: \t \n Famas: \t F F " << endl;
							}
						}
					}
					else
					{
						if (p == k1 || p == k3)
						{
							cout << "Puntos: \t P \n Famas: \t F " << endl;
						}
						else
						{
							if (p == k4)
							{
								cout << "Puntos: \t \n Famas: \t F F " << endl;
							}
							else
							{
								cout << "Puntos: \t \n Famas: \t F " << endl;
							}
						}
					}
				}
			}
			else
			{
				if (o == k1 || o == k2 || o == k4)
				{
					if (p == k1 || p == k2 || p == k3)
					{
						cout << "Puntos: \t P P \n Famas: \t " << endl;
					}
					else
					{
						if (p == k4)

						{
							cout << "Puntos: \t P \n Famas: \t F " << endl;
						}
						else
						{
							cout << "Puntos: \t P \n Famas: \t " << endl;
						}
					}
				}
				else
				{
					if (o == k3)
					{
						if (p == k2 || p == k1)
						{
							cout << "Puntos: \t P \n Famas: \t F " << endl;
						}
						else
						{
							if (p == k4)
							{
								cout << "Puntos: \t \n Famas: \t F F " << endl;
							}
							else
							{
								cout << "Puntos: \t \n Famas: \t F " << endl;
							}
							
						}
					}
					else
					{
						if (p == k3 || p == k2 || p == k1)
						{
							cout << "Puntos: \t P Famas: \t " << endl;
						}
						else
						{
							if (p == k4)
							{
								cout << "Puntos: \t \n Famas: \t F " << endl;
							}
							else
							{
								cout << "Puntos: \t \n Famas: \t " << endl;
							}
						}
					}
				}
			}
		}

	}

	contador++;

	if (n == k1 & n == k2 & o == k3 & p == k4)
	{
		cout << "Felicidades!! \n Lo logro en " << contador << " intentos " << endl;
		control - 1;
	}

	//while (control == 0);

	

	return 0;
}
