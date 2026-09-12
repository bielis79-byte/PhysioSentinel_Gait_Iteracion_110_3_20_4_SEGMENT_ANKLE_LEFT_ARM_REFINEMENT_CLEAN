# V110.3.20.4 · Segment architecture refinement

Conserva la arquitectura segmentaria principal V110.3.20.0. Cambios quirúrgicos:
- L/RHeel, L/RBigToe y L/RSmallToe pasan por el puente V104/V107 cuando existen.
- q7/q14 se retargetean por orientación distal Ankle→BigToe usando el Jacobiano SKEL real.
- Si no existe BigToe en un frame, no se inventa el tobillo: queda sin driver distal en ese frame.
- Brazo izquierdo q36..q42: filtro simétrico 7 puntos, preservación >=90% ROM y limitador robusto de salto.
- No se fuerza coordinación contralateral ni se copia el brazo derecho.
- Cadera, rodilla, pelvis, tronco y arquitectura 75F→mesh permanecen sin cambio conceptual.
