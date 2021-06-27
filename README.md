# NIST_XCOM_V4.xlam

NIST_XCOM_V4 is derived from the NIST XCOM web application used to calculate photon cross sections for scattering, photoelectric absorption and pair production, as well as total attenuation coefficients, for any element, compound (Z ≤ 100), at energies from 1 keV to 100 GeV.

Acknowledgement:

XCOM: Photon Cross Sections DatabaseNIST Standard Reference Database 8 (XGAM), M.J. Berger, J.H. Hubbell, S.M. Seltzer, J. Chang, J.S. Coursey, R. Sukumar, D.S. Zucker, and K. Olsen, NIST, PML, Radiation Physics Division

See https://dx.doi.org/10.18434/T48G6X for detailed information about XCOM

Tabulated XCOM data is used with permission

Installation:

Download NIST_XCOM_V4 to the folder where you normally store your Add-ins, usually C:/Users/*UserName*/AppData/Roaming/Microsoft/AddIns
Start Excel
in the **DEVELOPER** tab, click the *Add-Ins* icon, select Nist_Xcom_V4 from the Add-Ins List, click OK. An **ADD-INS** tab should appear in the Ribbon.

Main Macro:

Click the **ADD-INS** tab. There should be only one macro shown, *GetSpectrum*.
Clicking the *GetSpectrum* macro brings up a dialog that will report values and optionally produce a plot of tabulated values for the requested atom or formula and range of energies. Note that the formula format is Atom1:Count1:Atom2:Count2 ...  e.g. Ca:1:C:1:O:3 for CaCO3 calcium carbonate.

To use other functions:

Click the **FORMULAS** tab, click the *Insert Function* icon, scroll down and select the *X-ray Functions* category and select the function from the list.

Special Security Note:
Unfortunately, Excel macros have become a hacker tool for distributing malware. NIST_XCOM_V4.xlam is open source. Users are advised to install with Excel macros disabled and to verify that the underlying code is clean before enabling macros.


