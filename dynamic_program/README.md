## Dynamic Programming

Sequential problem(social planner):

w($k_0$)=max $\Sigma_{t=0}^{\infty} \beta^t U(f(k_t)-k_{t+1})$  
st 0≤$k_{t+1}$≤$f({k_t});$  
   $k_{t+1} \in K$;  
   $k_0~~given$;  
   $f(k_t)= F(k_t,1) + (1- \delta)k_t=k_{t+1}+c_t$ 
   


Bellman equation version:  
v(k)=max {$U(f(k)-k^{'})+\beta v(k^{'})$}  
st 0≤$k^{'}$≤$f(k);$  
   $k^{'}\in K$;  


- state variable: k
- control variable: $k^{'}$
- policy function: $k^{'}=g(k)$
- K={0.04,0.08,0.12,0.16,0.2};$\beta=0.6$;$U()=ln()$;$f()=()^{0.3}$ 

By contraction mapping theorem: $v^*$=w
_______________________

- $s_t=k_t$
- $a_t=k_{t+1}$
- $r(s_t,a_t)=U(f(k_t)-k_{t+1})$
- $a_t=\sigma(s_t)=g(s_t)$
- $(Tv)(s)= max_{a\in A(s)}\{r(s,a) + \beta v(a) \}$


