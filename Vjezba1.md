```cpp
#include <iostream>
using namespace std;

//void bubble_sort(int* p, int n) {
//	for (int i = 0;i < n;i++) {
//		for (int j = 0;j < n - 1;j++) {
//			if (*(p + j) > *(p + j + 1)) {
//				int pom = *(p + j);
//				*(p + j) = *(p + j + 1);
//				*(p + j + 1) = pom;
//			}
//		}
//	}
//}
//void selection_sort(int* p, int n) {
//	for (int i = 0;i < n;i++) {
//		int nm = i;
//		int t = i;
//		while (t < n) {
//			if (*(p + nm) > *(p + t))
//				nm = t;
//			t++;
//		}
//		int pom = *(p + nm);
//		*(p + nm) = *(p + i);
//		*(p + i) = pom;
//	}
//}
//void MuV_s(char* p) {
//	for (int i = 0;*(p + i) != '\0';i++) {
//		if (*(p + i) > 'Z') {
//			*(p + i) -= 'a' - 'A';
//		}
//	}
//}
//void ispis(char* p, int n) {
//	for (int i = 0;i < n;i++) {
//		cout << *p << " ";
//		p++;
//	}
//}

//int upis(int* p) {
//	int i = 0;
//	while(1){
//		cin >> *(p + i);
//		if (*(p + i) == 0)
//			return i;
//		i++;
//	}
//}
//int dijelitelj(int* p,int n) {
//	int br = 0;
//	int i = 1;
//	if (n == 0)
//		return 0;
//	while (i <= n) {
//		if (*(p + n - i) % *(p + n) == 0)
//			br++;
//		i++;
//	}
//	return br;
//}
//int naj_d(int* p, int n) {
//	int nj = 0;
//	int p_nj = 0;
//	for (int i = 0;i < n;i++) {
//		if (dijelitelj(p, i) > nj) {
//			nj = dijelitelj(p, i);
//			p_nj = i;
//		}
//	}
//	return p_nj;
//}

//void ispis(char* p) {
//    for (int i = 0;*(p + i) != '\0';i++)
//        cout << *(p + i) << " ";
//    cout << endl;
//}
//int duljina_s(char* p) {
//    int i = 0;
//    while (*(p + i) != '\0')
//        i++;
//    return i;
//}
//void preokret(char* p) {
//    for (int i = 0;i < (duljina_s(p) / 2);i++) {
//        char pom = *(p + i);
//        *(p + i) = *(p + duljina_s(p) - 1 - i);
//        *(p + duljina_s(p) - 1 - i) = pom;
//    }
//}

//void provjera_e(int* p, int* p1) {
//    for (int i = 0;i < 4*5;i+=5) {
//        int be = 0;
//        for (int br = 0;br < 3;br++) {
//            for (int j = 0;j < 5;j++) {
//                if (*(p + i + j) == *(p1 + br)) {
//                    be++;
//                    break;
//                }
//            }
//        }
//        cout << be << endl;
//    }
//}

//void ispis(char* p) {
//    for (int i = 0;*(p + i) != '\0';i++) {
//        cout << *(p + i) << " ";
//    }
//}
//int duljina(char* p) {
//    int i;
//    for (i = 0;*(p + i) != '\0';i++) {
//    }
//    return i;
//
//}
//void umetanje(char* p, char* p1, int n) {
//
//    int d = duljina(p);
//    int d1 = duljina(p1);
//    
//    for (int i = d;i >= n;i--) {
//        *(p + i + d1) = *(p + i);
//    }
//    for (int i = n;i < d1 + n;i++) {
//        *(p + i) = *(p1 + i - n);
//    }
//}

//void uk_ispis(int* p) {
//    for (int i = 0;i < 7 * 5 * 10;i += 5 * 10) {
//        for (int j = 0;j < 5 * 10;j += 10) {
//            for (int k = 0;k < 10;k++) {
//                cout << *(p + i + j + k) << " ";
//            }
//            cout << endl;
//        }
//        cout << endl;
//    }
//}
//int zaokruzi(float x) {
//    if ((x < 1) && (x != 0))
//        return 1;
//    if (x - int(x) >= 0.5)
//        return int(x) + 1;
//    return int(x);
//}
//void upisivanje(int* p, int oc) {
//    for (int i = 0;i < 10;i++) {
//        if (*(p + i) == 0) {
//            *(p + i) = oc;
//            break;
//        }
//    }
//}
//float prosjek(int* p) {
//    int suma = 0;
//    int br = 0;
//    for (int i = 0;i < 10;i++) {
//        if (*(p + i) != 0) {
//            suma += *(p + i);
//            br++;
//        }
//    }
//    if (br == 0)
//        return 0;
//    return suma / float(br);
//}
//void prosjek_sve(int* p) {
//    for (int i = 0;i < 5 * 10;i += 10) {
//        cout << prosjek(p + i) << endl;
//    }
//}
//void opci_uspjeh(int* p) {
//    int pomak_p = 10;
//    int pomak_u = 5 * pomak_p;
//
//    for (int i = 0;i < 7 * pomak_u;i += pomak_u) {
//        int suma = 0;
//        int br = 0;
//        for (int j = 0;j < 5 * pomak_p;j += pomak_p) {
//            suma += zaokruzi(prosjek(p + i + j));
//            if (prosjek(p + i + j) != 0)
//                br++;
//        }
//        if (br == 0)
//            cout << 0 << endl;
//        else
//            cout << suma / float(br) << endl;
//    }
//}

//void ispis(int* p) {
//    for (int i = 0;*(p+i)!=0;i++) {
//        cout << *(p + i) << " ";
//    }
//    cout << endl;
//}
//void del_parni(int* p) {
//    for (int i = 0;*(p + i) != 0;i++) {
//        int provjera = 1;
//        for(int j = 0;*(p+j+1)!=0;j++)
//            if (*(p + j) % 2 == 0) {
//                int pom = *(p + j);
//                *(p + j) = *(p + j + 1);
//                *(p + j + 1) = pom;
//                provjera = 0;
//            }
//        if (provjera)
//            return;
//    }
//    for (int i = 0;*(p + i) != 0;i++) {
//        if (*(p + i) % 2 == 0)
//            *(p + i) = 0;
//    }
//}

//void upisV(int* p) {
//    while (1) {
//        cin >> *p;
//        if (*p == 0)
//            return;
//        p++;
//    }
//}
//float prosjecnaV(int* p) {
//    float put = 0;
//    float vrijeme = 0;
//    for (int i = 0;*(p + i + 1) != 0;i++) {
//        int prosjecna = (*(p + i) + *(p + i + 1)) / 2;
//        put += prosjecna * 0.5;
//        vrijeme += 0.5;
//    }
//    return put / vrijeme;
//}

int zb_parnih(int* p, int n) {
    int zbroj = 0;
    for (int i = 0;i < n;i++) {
        if (*(p + i) % 2 == 0) {
            zbroj += *(p + i);
        }
    }
    return zbroj;
}
int broj_rijeci(char* p) {
    int br;
    if (*p == ' ')
        br = 0;
    else
        br = 1;
    for (int i = 0;*(p + i + 1) != '\0';i++) {
        if ((*(p + i) == ' ') && (*(p + i + 1) != ' ')) {
            br++;
        }
    }
    return br;
}
float br_slova_prosjecan(char* p) {
    int br = 0;
    for (int i = 0;*(p + i) != '\0';i++) {
        if (*(p + i) != ' ') {
            br++;
        }
    }
    return float(br) / broj_rijeci(p);
}
void ispis_rijeci(char* p) {
    bool provjera = false;
    if (*p != ' ')
        provjera = true;
    for (int i = 0;*(p + i + 1) != '\0';i++) {
        if (provjera == true) {
            int j;
            for (j = 0;*(p + j) != ' ';j++) {
                cout << *(p + j);
            }
            cout << endl;
            i += j;
            provjera = false;
        }
        if ((*(p + i) == ' ') && (*(p + i + 1) != ' ')) {
            int j;
            for (j = 1;*(p + i + j) != ' ';j++) {
                if (*(p + i + j) == '\0')
                    return;
                cout << *(p + i + j);
            }
            cout << endl;
            i += j - 1;
        }
    }
}

int main() {
    
    char rijec[] = "Jabuka   je   super   ";
    
    return 0;
}

```
