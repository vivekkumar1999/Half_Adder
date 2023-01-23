# Half_Adder
Design of Half Adder using verilog in Vivado



module half_adder(clr,a,b,sum,carry);
input a,b,clr ;
output sum,carry ;
wire w1,w2;
    and and1(w1,a,clr);  
    and and2(w2,b,clr);
    xor sum1(sum,w1,w2);
    and carry1(carry,w1,w2);
endmodule
