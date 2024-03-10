
This patch fixes a crash in oBG2 (v2.5.26498) related to TOT handling. Due to not properly initializing an important field, the game may randomly crash when attempting its first write to a save's TOT file, (this is usually during character creation for the character Biography / Name). This crash becomes nearly guaranteed under certain modded environments, such as using cnc-ddraw.
