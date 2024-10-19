module Carry_lookahead_tb ();
	reg [3:0] A,B;
	reg Cin;
	wire [3:0] Sum;
	wire Cout;
	
	Carry_lookahead DUT(.A(A),.B(B),.Cin(Cin),.Sum(Sum),.Cout(Cout));
	
	initial
	begin
		A = 4'b0000;
		B = 4'b0000;
		Cin = 1'b0;
		#10
		A = 4'b1001;
		B = 4'b0010;
		Cin = 1'b0;
		#10
		A = 4'b0010;
		B = 4'b0110;
		Cin = 1'b0;
		#10
		A = 4'b1110;
		B = 4'b1110;
		Cin = 1'b1;
		#10
		A = 4'b1111;
		B = 4'b1010;
		Cin = 1'b1;
		#10
		A = 4'b1010;
		B = 4'b1111;
		Cin = 1'b1;
		#10
		A = 4'b1000;
		B = 4'b0101;
		Cin = 1'b0;
		#10
		A = 4'b0110;
		B = 4'b1000;
		Cin = 1'b1;
		#20 $finish;
	end
	initial
	begin
		$monitor("A=%b | B=%b | Cin=%b | Sum=%b | Cout=%b",A,B,Cin,Sum,Cout);
	end 
endmodule
