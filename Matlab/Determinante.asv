%matriz a resolver (ejemplo)

A=[4 -5 2;1 -3 7;-2 6 4];

%Función que permite el calculo del determinante o Wroskiano de una matriz
function d=determinante(A)
n=1:size(A,1);
for k=1:size(A,1)
%La siguiente condición simplemente nos dice que si la matriz tiene un solo
%valor, es decir que sea 1x1, entonces el determinante es la misma matriz
    if size(A,1)==1
        d=A;
    else
        %Restricciones a tener en cuenta
        f=n(n~=1);
        c=n(n~=k);
        %Se calcula determinante de K que va a variar y se suman los
        %resultados:
        d(k)=((-1)^(1+k))*A(1,k)*determinante(A(f,c));
        d=sum(d);

%Para hallar determinante: en Command Window escribir det(A)
        
    end
end
end