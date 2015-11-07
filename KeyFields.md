Column   Name                  Examples - Description

1       UNIQUE\_NAME           mix10/bseywA - name used in all trial and training lists to identify the recording

2       DATABASE              FISHE1 FISHE2 MIX04 MIX05 MIX06 MIX08 MIX10 SWCELLP1 SWCELLP2 SWPH2 SWPH3 - database id

3       SPEAKER\_PIN           MIX100304 FISHE72815 SW1002 - speaker pin (unique across and within databases)

4       SESSION\_NAME          oczr - session name assigned in original database

5       CHANNEL               a,b,x - channel, x is used for mono waveforms

6       SESSION\_ID            mmsr\_20100126\_150751\_LDC\_83430\_mx6\_A\_int\_MIX120905 - original filename from which the waveform was cut appended with channel, speech style and speaker id to make it unique

7       GENDER                f,m - gender

8       YEAR\_OF\_BIRTH         1978 - year of birth of speaker in signal

9       YEAR\_OF\_RECORDING     2003 - year of recording of signal

10       AGE                   41 - age of speaker in signal

11       SPEECH\_TYPE           tel, int - telephone conversation or interview

12       CHANNEL\_TYPE          phn, MIX10-mic02 - type of recording channel, phn for telephone channel, database\_name-microphone\_id for microphone channels

13       NOMINAL\_LENGTH        300, 500 - duration in seconds derived from TASK, 5minutes = 300, but also 8min, 10sec ...

14       LANGUAGE              ENG, ARA, RUS - normalized to a set of three letter names

15       NATIVE\_LANGUAGE       English, German/Arabic - as declared by speaker

16       VOCAL\_EFFORT          NA, normal, high, low - vocal effort level