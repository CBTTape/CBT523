# CBT523
Converted to GitHub via [cbt2git](https://github.com/wizardofzos/cbt2git)

This is still a work in progress. 
Due to amazing work by Alison Zhang and Jake Choi repos are no longer deleted.

```
//***FILE 523 is from Paul Dion and contains an SMF record          *   FILE 523
//*           selection program of great generality.  Records can   *   FILE 523
//*           be pulled from the currently active SMF dataset, as   *   FILE 523
//*           well as from SMF archive datasets.                    *   FILE 523
//*                                                                 *   FILE 523
//*           email:  pdion@canada.com                              *   FILE 523
//*                                                                 *   FILE 523
//*           Fixed by  R.W. Suhr          (see members $$NOTEx)    *   FILE 523
//*           email:  RSuhr@iot.IN.gov                              *   FILE 523
//*                                                                 *   FILE 523
//*      SMFSLCT Index                                              *   FILE 523
//*                                                                 *   FILE 523
//*      The following is a one-line description of the             *   FILE 523
//*      contents of this library:                                  *   FILE 523
//*                                                                 *   FILE 523
//*      $$$$$$IX - Index: this is it                               *   FILE 523
//*      $$$$$DOC - A brief overview of the SMFSLCT program         *   FILE 523
//*      $$$$INST - Sample Assemble and Link JCL                    *   FILE 523
//*      $$$$SAMP - Sample execution JCL                            *   FILE 523
//*      $$$CHANG - Changes with this version                       *   FILE 523
//*      SMFSLCT  - Assembler source                                *   FILE 523
//*                                                                 *   FILE 523
//*                     S  M  F  S  L  C  T                         *   FILE 523
//*                                                                 *   FILE 523
//*       This program will read SMF data (from the MAN             *   FILE 523
//*      datasets or output from IFASMFDP), and will select         *   FILE 523
//*      records according to user specified criteria.              *   FILE 523
//*      Records can be selected by date and time, by record        *   FILE 523
//*      type (and /or subtype), by Jobname, or by data at an       *   FILE 523
//*      offset within the record. Records must meet date/time      *   FILE 523
//*      and record type criteria before being eligible for         *   FILE 523
//*      selection, as determined by Jobname and/or data            *   FILE 523
//*      specifications.                                            *   FILE 523
//*                                                                 *   FILE 523
//*       By default, any records selected from the input           *   FILE 523
//*      will be printed to SYSPRINT, unless 'PRINT=NO' is          *   FILE 523
//*      specified in the SYSIN control cards. If SYSUT2 is         *   FILE 523
//*      present, the selected input records will also be           *   FILE 523
//*      written to it.                                             *   FILE 523
//*                                                                 *   FILE 523
//*       Multiple output files with different selection            *   FILE 523
//*      criteria can be produced in one run of SMFSLCT. The        *   FILE 523
//*      output DDNames and selection criteria are specified        *   FILE 523
//*      in the control cards in SYSIN.                             *   FILE 523
//*                                                                 *   FILE 523
//*       Two user-written exits can be used with SMFSLCT -         *   FILE 523
//*      the first is given control after an SMF record is          *   FILE 523
//*      read, and the second after an SMF record has been          *   FILE 523
//*      selected.                                                  *   FILE 523
//*                                                                 *   FILE 523
//*      Input:                                                     *   FILE 523
//*          SYSUT1   - SMF dataset - either the output from        *   FILE 523
//*                     IFASMFDP or one of the SYS1.MAN             *   FILE 523
//*                     datasets. If this DDName is not             *   FILE 523
//*                     allocated, it will be dynamically           *   FILE 523
//*                     allocated to the active SMF dataset.        *   FILE 523
//*                                                                 *   FILE 523
//*          SYSIN    - Control cards (see below).                  *   FILE 523
//*                                                                 *   FILE 523
//*      Output:                                                    *   FILE 523
//*          SYSPRINT - Error messages, selected SMF records.       *   FILE 523
//*          SYSUT2   - optional, selected SMF records.             *   FILE 523
//*                                                                 *   FILE 523
//*      Attributes:                                                *   FILE 523
//*          Re-entrant, Reuseable, Refreshable, Not Authorized,    *   FILE 523
//*          AMODE(31), RMODE(ANY)                                  *   FILE 523
//*                                                                 *   FILE 523
```
