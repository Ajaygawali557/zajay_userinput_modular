# zajay_userinput_modular


*--- User Input
PARAMETERS: p_num1 TYPE i,
            p_num2 TYPE i.

*--- Variable for result
DATA: gv_sum TYPE i.

*--- Main Logic
START-OF-SELECTION.

  PERFORM calculate_sum.
  PERFORM display_output.

*--- FORM to calculate sum
FORM calculate_sum.
  gv_sum = p_num1 + p_num2.
ENDFORM.

*--- FORM to display result
FORM display_output.
  WRITE: 'The sum of', p_num1, 'and', p_num2, 'is', gv_sum.
ENDFORM.
