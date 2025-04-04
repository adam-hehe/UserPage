# Adam Connor's Website

## About Me
Hi, my name is Adam Connor and I'm a second year **Computer Science student at UC San Deigo** 
and an active member of **SHPE** (Society of Hispanic Professional Engineers). 

![Alt](https://studyabroad.ucsd.edu/_images/majors-maps/major-modules/cse-building.jpg)

### Relevant Coursework
- [x] Advanced Data Structures
- [x] Design and Analysis of Algorithms
- [x] Computer Organization and Systems Programming
- [x] Software Tools and Techniqes Lab
- [x] Theory of Computation
- [x] Mathmatics for Algorithms and Systems
- [x] Linear Algebra
- [ ] Statistical Methods
- [ ] Software Engineering

> Software Engineering and Statistical Methods to be completed 6/14/2025

### Interests
Some of my interest within the field include:
1. Artificial Intellegence and Machine Learning
2. Software Development
3. Cypersecurity
4. Systems and Low-Level Programming

![Alt](https://www.lawrence.edu/sites/default/files/styles/medium_16_9/public/2022-01/snapshot_compscience.jpg?h=8abcec71&itok=ERJ7l-gs)

### Languages
Languages I'm have proficent coding experience in include: 
- Java
- Python
- C, C#, C++
- Javascript

### Project Example

Below is a sample encryption algorithm built in C that uses bitwise manipulation

``` C
int
ecrypt(unsigned char *inbuf, unsigned char *bookbuf, int cnt)
{
    if (cnt <= 0) return 0;
    unsigned char *inptr = inbuf;
    unsigned char *bookptr = bookbuf;
    unsigned char currB;
    for(int i = 0; i < cnt; i++) {
        currB = *inptr;
        currB = (currB >> 4) | (currB << 4);
        currB = ((currB & 0xCC) >> 2) | ((currB & 0x33) << 2);
        currB = ((currB & 0xAA) >> 1) | ((currB & 0x55) << 1);
        
        currB = currB ^ *bookptr;
        *inptr = currB;
        
        inptr++;
        bookptr++;
    }
    return cnt;
}
```


### Appendix

*Linkedin Profile [here](https://www.linkedin.com/in/adam-connor-8708a5282/).*

Go to [README](./README.md)

[Back to Top](#about-me)

