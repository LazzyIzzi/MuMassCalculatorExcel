# NIST_XCOM.xlam

NIST_XCOM is derived from the NIST XCOM web application used to calculate photon cross sections for scattering, photoelectric absorption and pair production, as well as total attenuation coefficients, for any element, compound (Z ≤ 100), at energies from 1 keV to 100 GeV.

Acknowledgement:

XCOM: Photon Cross Sections DatabaseNIST Standard Reference Database 8 (XGAM), M.J. Berger, J.H. Hubbell, S.M. Seltzer, J. Chang, J.S. Coursey, R. Sukumar, D.S. Zucker, and K. Olsen, NIST, PML, Radiation Physics Division

See https://dx.doi.org/10.18434/T48G6X for detailed information about XCOM

Tabulated XCOM data is used with permission
<br>See https://lazzyizzi.github.io/CT_ReconPages/XrayCalculatorExcel.html for additional installation and use information.
Installation:

Download NIST_XCOM.xlam to the folder where you normally store your Add-ins, usually C:/Users/*UserName*/AppData/Roaming/Microsoft/AddIns. 
Start Excel. 
In the **DEVELOPER** tab, click the *Add-Ins* icon, select Nist_Xcom from the Add-Ins List, click OK. An **ADD-INS** tab should appear in the Ribbon.

**Macros:**

Click the **ADD-INS** tab. There should be two macros shown in the ToolBar Commands, *GetSpectrum* and *BeamHardening*.
Clicking the *GetSpectrum* macro brings up a dialog that will report values and optionally produce a plot of tabulated values for the requested atom or formula and range of energies. Note that the formula format is Atom1:Count1:Atom2:Count2 ...  e.g. Ca:1:C:1:O:3 for CaCO3 calcium carbonate.

Clicking the *BeamHardening* runs a macro that builds a 1D model of a radiography system. The macro shows a dialog that asks for data about the x-ray source, x-ray filter, sample size and composition, detector screen, and energy range to plot. After entering the data, Click **Update Plot** to show a plot of the x-ray intensity vs energy at five points along the x-ray path. The percent beam hardening and photon efficiency are displayed in the plot title. Adjust the x-ray source and filter so that to an acceptable level of beam hardening and photon efficiency. Alternatively, click the **Optimize** button to run the Solver.

BeamHardening Notes:
<ul>
<li>The results of this macro are meant to guide source and filter selection and may differ from that observed from an actual x-ray system.</li>
<li>The Kramers equation is used to compute source intensities.  Characteristic emission lines and source configuration are neglected.</li>
<li>The detector is "ideal" in that the intensity absorbed by the detector screen material is recorded. There are no adjustments for collection efficiency, fluorescent yield, amplification etc.</li>
</ul>

**Functions:**

Click the **FORMULAS** tab, click the *Insert Function* icon, scroll down and select the *X-ray Functions* category and select a function from the list to display an input dialog.

For more information open LazzyIzzi's [X-ray Calculator Excel](https://lazzyizzi.github.io/CT_ReconPages/XrayCalculatorExcel.html)  project in a new tab or window.


**Special Security Note:**
Unfortunately, Excel macros have become a hacker tool for distributing malware. NIST_XCOM.xlam is open source. Users are advised to install with Excel macros disabled and to verify that the underlying code is clean before enabling macros.


