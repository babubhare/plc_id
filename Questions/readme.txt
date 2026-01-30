create an table for 3 lane traffic with 3 lights following Indian standard. At any point of time there should be only one green. And Green can be active for 30 secs and Yellow can be active for 10 seconds.
The Green duration is seconds; Yellow duration is 10s seconds. Please use accronyms for Red as R, Yellow as Y & Green as G. Like G1, Y1, R1 etc. Yellow can transition to Green Only as per Indian standard. At any point of time One Green should be on. But make sure any green should be ON in any state.
Transition to Green should be with Yellow

3 Lane Indian
State,Time Interval (Sec),Duration,Lane 1 (L1),Lane 2 (L2),Lane 3 (L3),Description
1,00 - 20,20s,G1,R2,R3,Lane 1 is flowing freely.
2,20 - 30,10s,G1,Y2,R3,Lane 1 is ending. Lane 2 gets ready (Yellow).
3,30 - 50,20s,R1,G2,R3,Lane 1 Stops. Lane 2 is flowing freely.
4,50 - 60,10s,R1,G2,Y3,Lane 2 is ending. Lane 3 gets ready (Yellow).
5,60 - 80,20s,R1,R2,G3,Lane 2 Stops. Lane 3 is flowing freely.
6,80 - 90,10s,Y1,R2,G3,Lane 3 is ending. Lane 1 gets ready (Yellow).

***************************************************************************************************************************************************************************************************************************
3 Lane International

State,Time,Lane 1,Lane 2,Lane 3,Status Description
1,0s - 10s,G1,R2,Y3,L1 Starts. L3 Clearance (Y$\rightarrow$R).
2,10s - 20s,G1,R2,R2,L1 Solo Flow. (Middle of cycle).
3,20s - 30s,G1,Y2,R3,L1 Ends. L2 Get Ready (R$\rightarrow$Y).
4,30s - 40s,Y1,G2,R3,L2 Starts. L1 Clearance (Y$\rightarrow$R).
5,40s - 50s,R1,G2,R3,L2 Solo Flow. (Middle of cycle).
6,50s - 60s,R1,G2,Y3,L2 Ends. L3 Get Ready (R$\rightarrow$Y).
7,60s - 70s,R1,Y2,G3,L3 Starts. L2 Clearance (Y$\rightarrow$R).
8,70s - 80s,R1,R2,G3,L3 Solo Flow. (Middle of cycle).
9,80s - 90s,Y1,R2,G3,L3 Ends. L1 Get Ready (R$\rightarrow$Y).


***************************************************************************************************************************************************************************************************************************
create an table for 4 lane traffic with 3 lights following Indian standard. At any point of time there should be only one green. And Green can be active for 30 secs and Yellow can be active for 10 seconds.
The Green duration is seconds; Yellow duration is 10s seconds. Please use accronyms for Red as R, Yellow as Y & Green as G. Like G1, Y1, R1 etc. Yellow can transition to Green Only as per Indian standard. At any point of time One Green should be on. But make sure any green should be ON in any state.
Transition to Green should be with Yellow. The cycle should repeat.

4Lane Indians are

Phase,Duration,Lane 1,Lane 2,Lane 3,Lane 4
Time Interval,Duration,Lane 1,Lane 2,Lane 3,Lane 4,Active Green
0 – 20s,20s,G1,R2,R3,R4,Lane 1
20 – 30s,10s,G1,Y2,R3,R4,Lane 1
30 – 50s,20s,R1,G2,R3,R4,Lane 2
50 – 60s,10s,R1,G2,Y3,R4,Lane 2
60 – 80s,20s,R1,R2,G3,R4,Lane 3
80 – 90s,10s,R1,R2,G3,Y4,Lane 3
90 – 110s,20s,R1,R2,R3,G4,Lane 4
110 – 120s,10s,Y1,R2,R3,G4,Lane 4
***************************************************************************************************************************************************************************************************************************
create an table for 4 lane traffic with 3 lights following International standard. At any point of time there should be only one green. And Green can be active for 30 secs and Yellow can be active for 10 seconds.
The Green duration is 30 seconds; Yellow duration is 10s seconds. Please use accronyms for Red as R, Yellow as Y & Green as G. Like G1, Y1, R1 etc. Yellow can transition to Green Or Red as per International standard. At any point of time One Green should be on. But make sure any green should be ON in any state.
Transition to Green should be with Yellow. At any point the transition to Red should be with Yellow. The cycle should repeat. Allow overlapping yellow. But make sure any green should be ON in any state

4Lane Indians are
State,Duration,Lane 1,Lane 2,Lane 3,Lane 4,Logic Description
Stage,Time Interval,Lane 1,Lane 2,Lane 3,Lane 4,Status Description
1,0s – 30s,G1,R2,R3,R4,Lane 1 Green solo
2,30s – 40s,Y1,G2,R3,R4,L1 clears / L2 starts Green
3,40s – 60s,R1,G2,R3,R4,Lane 2 Green solo (cont.)
4,60s – 70s,R1,Y2,G3,R4,L2 clears / L3 starts Green
5,70s – 90s,R1,R2,G3,R4,Lane 3 Green solo (cont.)
6,90s – 100s,R1,R2,Y3,G4,L3 clears / L4 starts Green
7,100s – 120s,R1,R2,R3,G4,Lane 4 Green solo (cont.)
8,120s – 130s,G1,R2,R3,Y4,L4 clears / L1 starts Green
9,130s – 160s,G1,R2,R3,R4,Cycle repeats (L1 Green cont.)