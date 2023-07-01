# Wallet With Proteous
Digital Wallet

In this problem, I design a simple digital wallet that can be activated with a password and allows users to deposit or withdraw money. The circuit will be implemented as a sequential circuit, utilizing the necessary clock pulse provided by the input clk.

For the security of the wallet, a 4-bit password is considered. By enabling the ch_pass signal, the user can enter a 4-bit value as the software password. The stored money value will be a 7-bit number (ranging from 0 to 127). This value is initialized to 0 and can be displayed at any time through the output out.

How the wallet works: Upon entering the correct 4-bit password, the En_out output becomes 1, allowing the user to perform either a deposit or a withdrawal operation. If the password is entered incorrectly, the En_out output becomes 0, and no operations can be performed on the stored money value. The deposit operation is performed by providing the desired money value in the 7-bit input and setting the add/sub signal to 0. In this case, if the password is correct, pressing the apply button will add the input value to the previous value and store it in the wallet. The withdrawal operation is performed by providing the desired money value in the 7-bit input and setting the add/sub signal to 1. In this case, if the password is correct, pressing the apply button will subtract the input value from the previous value and store it in the wallet. When the Reset signal becomes 1, the money value in the wallet should be set to zero.
