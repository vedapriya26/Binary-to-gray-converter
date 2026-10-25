# Binary-to-gray-converter
module bin2gray #(parameter n=8)
(input [n-1:0]bin,output [n-1:0]gray);
genvar i;
generate
for(i=0;i<n-1;i=i+1) begin:bin2gray
     assign gray[i]=bin[i]^bin[i+1];
   end
endgenerate
   assign gray[n-1]=bin[n-1];
endmodule
