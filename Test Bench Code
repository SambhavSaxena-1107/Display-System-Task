// Example uses for $display system task
module test_display;
  
  reg[8*200:0] my_string;
  reg[15:0] my_number;
  real my_time;
  
  my_design my_design();
  
  initial begin
//Display string
    $display("Hello World!");
    my_string = "This is Verilog";
    $display("The String is %0s",my_string);
    
//Display decimal, binary, hex numbers
    my_number=8'h1a;
    $display("Decimal: %0d", my_number);
    $display("Binary: %0b", my_number);
    $display("Hex: %0h", my_number); 
    
//Display hierarchicalname
    $display("I'm at %m");
    my_design.print;
 
//Display time
    my_time = 123;
    $display("Current time %0t, and dummy time %0t", $time, my_time);
    #11;
    $display("Current time %0t, and dummy time %0t", $time, my_time);
    
//Long message display
    my_string = {"Module Declaration Defines the module's name and ports.\n Ports define the interface of the module.\n Data Types define different signals and variables."};
    $display("%0s %0s and %0t %0d", my_string, "string", $time, my_number);
    
  end
endmodule
