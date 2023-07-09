
#BasicsOfEEE #DCMotorCurrent #DCMotorStarter #SeriesMotor

We know, the voltage equation of the DC Motor is 
$$V=E_B+I_a\cdot R_a$$

So,
$$I_a=\frac{V-E_B}{R_a}$$

Also we know that 
$$
\begin{align*}
	E_b&=\frac{\phi Zn}{60}\\
	E_b&\propto \phi N
\end{align*}
$$
Where, $E_b$ = ***TODO***:

When starting the motor, $N=0, E_b=0$
$$\begin{align*}\therefore I_a &= Starting Current = I_{as}\\

I_{as} &= \frac{V}{R_a}; R_a \approxeq 0.5 - 1\text { } \ohm 
	\end{align*}
$$

if $V = 230V$ , $R_a=0.5\ohm$
$$I_{as} = \frac {230}{0.5} = 460 A >> I_\text{rated}$$

#DCMotorStarter 
The purpose of a starter is to limit to starting current 