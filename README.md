# Non-Divisible-Subset

For any number K, the sum of 2 values (A & B) is evenly divisible by K if the sum of the remainders of A/K + B/K is K.

I Inititalized k size array with 0 to store frequency of remainders for all m = s[i]%k;

why k=size? because if we divide by k, the remainder are always less than k;

how to store the frequency?

for (int i=0;i<s.size();i++)
{
    m=s[i]%k;
    modulo[m]++;
}

How to compare two values:

max(modulo[i],modulo[k-i]);


