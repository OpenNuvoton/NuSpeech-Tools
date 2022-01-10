All installers are zipped with password: 123456

-------------
N588L SDS V1.06.000 SP2
-------------
Based on N588L V1.06.000 SP1 and add the following issues.

[Modification]
+ Improvement on UIO code-generation
 
[Bug-Fixed]
+ For these equations with silence inside, if we do not use these equations in user program, it will lead to linking error.

-------------
N588L SDS V1.06.000 SP1
-------------
Based on N588L V1.06.000 and add the following issues.

[Features]
 + HW PWM Frequency show real frequency instead of clock source.
 
[Bug-Fixed]
 + FW PWM Frequency option didn't contain in modification list so it do not update if it was changed individually
 + Apply HW PWM Frequency option to codgen.
 + Allow to type '-' (hyphen) in project name(#0003184)

-------------
N588L SDS V1.06.000
-------------
Based on SDS V1.05.000 and add the following issues.

[Features]
+ Support play by index function.
+ Support to apply the property about shift sample position on UltraIO file.