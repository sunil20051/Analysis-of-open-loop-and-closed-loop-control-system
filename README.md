 # Analysis-of-open-loop-and-closed-loop-control-system
## Aim :
  To analyse the open loop and closed loop system having G(S)=1/(S^2+10S+20)  when an unit step input is applied using MATLAB.
## Apparatus Required:
  Computer with MATLAB software
## Theory
  ### Open loop control system
  In this system, the output doesn’t change the action of the control system. It doesn’t have any feedback. It is very simple, needs low maintenance, quick operation, and cost-effective. The accuracy of this system is low and less dependable.
  <img width="652" height="175" alt="image" src="https://github.com/user-attachments/assets/0a9d8129-eb64-40bb-8efd-434edcb2bd5a" />
 ### Closed loop control System
The closed-loop control system can be defined as the output of the system that depends on the input of the system. This control system has one or more feedback loops among its input & output. This system provides the required output by evaluating its input. This kind of system produces the error signal and it is the main disparity between the output and input of the system.
                     <img width="508" height="220" alt="image" src="https://github.com/user-attachments/assets/ad4b9b9e-bf06-4108-a4c0-5320be064b1f" />

Consider a system having plant G(S)=  1/(S^2+10S+20), H(S) = 1(negative unity feedback system) and Controller C(S) = 300.
C(S) and G(S) are in series, 300/(S^2+10S+20)
300/(S^2+10S+20) and H(S) are in negative feedback.
Therefore, Closed loop transfer function, (C(S))/(R(S))=300/(S^2+10S+320)
## Program: 
### Open loop System
num[1] <brk>
den[1 10 20] <brk>
sys=tf(num,den) <brk>
step(sys )<brk>

### Closed loop System
num=[300]<brk>
den=[1 10 320]<brk>
sys=tf(num,den)<brk>
step(sys)<brk>

## Procedure:
	Open MATLAB software
	Open a new script file.
	Type the program.
	Save and Execute the program.
	Analyse the result.
## Output:
### Open Loop System

<img width="1920" height="1200" alt="Screenshot 2025-09-24 093828" src="https://github.com/user-attachments/assets/3f3c34ea-c446-4afe-8a7c-33aa6dba8510" />

### Closed Loop System
<img width="792" height="472" alt="image" src="https://github.com/user-attachments/assets/20598693-84fc-4b0e-9111-d31791cd5ad1" />

## Result:
Thus the open loop and closed loop system are analysed and the following conclusions are arrived.
### Open loop system
Steady State Error =0.95 <brk>
Settling Time = 2.5<brk>
### Closed loop System
Steady State Error = 0.05 <brk>
Settling Time = 1.23 <brk>





