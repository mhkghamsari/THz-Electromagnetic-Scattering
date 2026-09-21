Main common settings

•	2D electromagnetic model.

•	TM polarization.

•	Plane wave incident at \\(30^\\circ\\).

•	Four dielectric layers, each 1.25 mm thick.

•	Relative permittivities: 3.55, 4, 5, and 6.

•	Material losses are included.

•	\\(S\_{11}\\) magnitude and phase are referenced to the top surface, \\(y=0\\).





PML: 300 GHz versus 500 GHz

The geometry, materials, excitation, PML thickness, and \\(S\_{11}\\) calculation are identical.

Only these differ:

•	Operating frequency.

•	The 500 GHz model has a finer mesh because its wavelength is shorter.

•	Consequently, the 500 GHz file requires more memory.







Periodic model	                                   PML model

Uses a small 0.5 mm repeating cell	Uses the complete 50 mm structure

Periodic boundaries on the sides	PML absorbing regions around the structure

Excited using a periodic port	Excited using a background plane wave

Uses COMSOL’s port \\(S\_{11}\\)	Calculates \\(S\_{11}\\) by projecting the scattered field

Best for an infinite smooth surface	Appropriate for a finite rough surface



The COMSOL model contains:

•	Normalized scattered-field magnitude versus −80° to +80°.

•	Scattered-field phase versus angle.

•	Complex scattered electric field at a reference distance of 1 m.

•	2D RCS/scattering width versus angle.

•	A prepared CSV export.

•	A verification evaluation at +30°.



After simulation, open Results and use:

1\.	Angular Scattered Field Magnitude (dB)

2\.	Angular Scattered Field Phase

3\.	2D RCS versus Observation Angle

4\.	Export Angular Scattering CSV



Angles are measured from the upward surface normal; the specular reflection is at \\(+30^\\circ\\).

