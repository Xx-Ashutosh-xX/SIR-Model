# SIR-Model
Analysis of Covid-19 Spread in West Bengal, India

Epidemiology Report on SARS-COV-2              West Bengal, India
-By Ashutosh Saxena & Shantanu Mehra

SIR Model: - 
The SIR Model is one of the simplest compartmental models, and many models are derivatives of this basic form. The model consists of three compartments: S for the number of Susceptible, I for the number of Infectious, and R for the number of Recovered or deceased (or immune) individuals.

Variables Used: -
N: -     Total population
S(t): - Number of people susceptible on day t
I(t): -   Number of people infected on day t
R(t): - Number of people recovered on day t
β: -    Expected amount of people an infected person infects per day
D: -     Number of days an infected person has and can spread the disease
γ: -     The proportion of infected recovering per day (γ = 1/D)
R₀: -   The total number of people an infected person infects (R₀ = β / γ)
L: -     Days after the start of outbreak, lockdown was imposed

Equations & Initial Variables Used:

	Ro=(N*ln⁡(□(S2/S1)))/((∆I+ ∆S) )                         

	dS/dt= -β*I*S/N

	dI/dt= β*I*S/N- γ*I

	dR/dt= γ*I
Figure-1
The High Inaccuracy observed here in the model is due to the fact that the model here uses R₀ = 2.79 which we have taken as basic reproductive number for SARS-COV-2 
(source = https://academic.oup.com/jtm/article/27/2/taaa021/5735319) i.e. if NO precautions were implemented by government and any preventive measures such as social distancing were not adhered to ,similar situation may have been observed.

Predictions in accordance with SIR Model (Actual observed values may be in vicinity**): -
	Highest Number of Infected that may be Observed = 25,132,495 on 105th day from the start of Epidemic.
	Total Number of Recovered that may be Observed = 84,494,335 at the end of the Epidemic
	Duration of Epidemic = 433 days
 
Figure-2

Implementation of lockdown has significantly brought down the numbers of max infected, but a downside being the predicted duration of epidemic has increased considerably from 433 to 592 days. 
The R₀ = 1.669787 for fitting the data is calculated using the following equation 
Ro=(N*ln⁡(□(S2/S1)))/((∆I+ ∆S) )   at each day and averaging over the time period.             

Predictions in accordance with SIR Model (Actual observed values may be in vicinity**): -

	Highest Number of Infected to be Observed = 8,593,224 on 220th day of the Epidemic
	Total Number of Recovered to be Observed = 61,864,404 at the end of the Epidemic
	Duration of Epidemic = 592 days
	16,535,332‬ number of infections may be avoided during the entire duration of epidemic, if the pace of spread of virus remains the same. 


Limitations of the model: -
	Over-Simplified
	Assumes that individual characteristics of immunity, susceptibility, and ability to recover, are essentially the same for all members of the population.
	It is assumed that the transmission rate remains constant throughout the period of pandemic.
	Assumes recovered individual has become immune to epidemic.






