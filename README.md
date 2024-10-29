module fa(a,b,c,sum,carry);
input a,b,c;
output sum,carry;
wire x1,x2,x3;
xor(x1,a,b);
and(x3,a,b);
xor(sum,x1,c);
and(x2,x1,c);
or(carry,x2,x3);
endmodule
