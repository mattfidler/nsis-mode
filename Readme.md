#  NSIS-mode
 Matthew L. Fidler
## Library Information
 __nsis-mode.el__ --- NSIS-mode

- __Filename__ --  nsis-mode.el
- __Description__ --  NSIS mode
- __Author__ --  Matthew L. Fidler
- __Maintainer__ --  Matthew L. Fidler
- __Created__ --  Tue Nov 16 15:48:02 2010 (-0600)
- __Version__ --  0.45
- __Last-Updated__ --  Mon Jul 08 21:05:17 2013 (+0100)
- __By__ --  Jan T. Sott
- __Update #__ --  1479
- __URL__ --  http:__github.com_mlf176f2_nsis-mode
- __Keywords__ --  NSIS
- __Compatibility__ --  Emacs 23.2

## Possible Dependencies

  None

A major mode for editing nsis files

## Installation

Put this `nsis-mode` the load path, then add the following to your Emacs:

 (autoload 'nsis-mode "nsis-mode" "NSIS mode" t)

 (setq auto-mode-alist (append '(("\\.\\([Nn][Ss][Ii]\\)$" .
                                  nsis-mode)) auto-mode-alist))

 (setq auto-mode-alist (append '(("\\.\\([Nn][Ss][Hh]\\)$" .
                                  nsis-mode)) auto-mode-alist))



## History

- __08-Jul-2013__ --   Added new NSIS 3.0a0 commands, sorted command list. (Jan T. Sott)
- __20-Aug-2012__ --   Added nsis-indent-level to allow customization of indentation. (Matthew L. Fidler)
- __08-Jun-2012__ --   Changed _ to syntax class (Matthew L. Fidler)
- __16-May-2012__ --   Added label indentation support for labels of the form "label_${ONE}:" (Matthew L. Fidler)
- __16-May-2012__ --   Fixed random hang (Matthew L. Fidler)
- __16-May-2012__ --   Attempted to fix random hangs. It could be due to indentation infinite loop, so made sure (bobp) is always checked at the beginning of the line. (Matthew L. Fidler)
- __01-Mar-2012__ --   Added website. (Matthew L. Fidler)
- __01-Mar-2012__ --   Bug fix for syntax table. (Matthew L. Fidler)
- __19-Dec-2011__ --   Looks for makensis if can't find in program files. (Matthew L. Fidler)
- __19-Dec-2011__ --   Added .nsi and .nsh autoload (Matthew L. Fidler)
- __07-Feb-2011__ --   Added check to make sure compile went OK before launching executable. (Matthew L. Fidler)
- __25-Jan-2011__ --   Added more explicit setup instructions (Matthew L. Fidler)
- __06-Dec-2010__ --   Changed comment start and comment stop to single line semi-colons (Matthew L. Fidler)
- __06-Dec-2010__ --   Made nsis-yas-description not depend on finding MUI<ul>FUNCTION<_ul>DESCRIPTION<ul>BEGIN. If MUI<_ul>DESCRIPTION_TEXT is found, insert there. (Matthew L. Fidler)
- __06-Dec-2010__ --   Updated indentation line function (bug-fix) (Matthew L. Fidler)
- __23-Nov-2010__ --   Macros that end with END or BEGIN are indentation keywords. (Matthew L. Fidler)
- __23-Nov-2010__ --   Changed indentation routine (bugfix)  ()
