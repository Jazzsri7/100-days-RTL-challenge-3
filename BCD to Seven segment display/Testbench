module BCD_Binary_tb();
reg [3:0] binary;
wire [6:0] seg;
integer i;

BCD_Binary DUT(.binary(binary),.seg(seg));

initial
begin
	
	for(i=0;i<10;i=i+1)
	begin
		binary=i;
		#20;
	end
	#20 $finish;
end

initial 
begin
	$monitor("value of abcdefg=%b",seg);
end
endmodule
