#### GO TO *[HOME PAGE](index.md)*

# Basic commands


      ipconfig (To check IP)
      dir (equivalent to ls in Linux)
      
      PS C:\Users\pyelgoi> $PSversiontable

          Name                           Value
          ----                           -----
          PSVersion                      5.1.14393.2214
          PSEdition                      Desktop
          PSCompatibleVersions           {1.0, 2.0, 3.0, 4.0...}
          BuildVersion                   10.0.14393.2214
          CLRVersion                     4.0.30319.42000
          WSManStackVersion              3.0
          PSRemotingProtocolVersion      2.3
          SerializationVersion           1.1.0.1
          
       You can pipe this information and use other commands, you can get what Methods and propertoies it has
       
     PS C:\Users\pyelgoi> $PSVersionTable | Get-Member
     TypeName: System.Collections.Hashtable

        Name              MemberType            Definition
        ----              ----------            ----------
        Add               Method                void Add(System.Object key, System.Object value), void IDictionary.Add(Syste...
        Clear             Method                void Clear(), void IDictionary.Clear()
        Clone             Method                System.Object Clone(), System.Object ICloneable.Clone()
        Contains          Method                bool Contains(System.Object key), bool IDictionary.Contains(System.Object key)
        ContainsKey       Method                bool ContainsKey(System.Object key)
        ContainsValue     Method                bool ContainsValue(System.Object value)
        CopyTo            Method                void CopyTo(array array, int arrayIndex), void ICollection.CopyTo(array arra...
        Equals            Method                bool Equals(System.Object obj)

      dir | get-member
      
      Store a value 
          
          PS C:\Users\pyelgoi> 1+2
          3
          PS C:\Users\pyelgoi> $a = 1+2
          PS C:\Users\pyelgoi> $a
          3
          PS C:\Users\pyelgoi> $a | get-member


           TypeName: System.Int32

        Name        MemberType Definition
        ----        ---------- ----------
      CompareTo   Method     int CompareTo(System.Object value), int CompareTo(int value), int IComparable.CompareTo(Syste...
      Equals      Method     bool Equals(System.Object obj), bool Equals(int obj), bool IEquatable[int].Equals(int other)
      GetHashCode Method     int GetHashCode()
      GetType     Method     type GetType()
      GetTypeCode Method     System.TypeCode GetTypeCode(), System.TypeCode IConvertible.GetTypeCode()
      ToBoolean   Method     bool IConvertible.ToBoolean(System.IFormatProvider provider)
      ToByte      Method     byte IConvertible.ToByte(System.IFormatProvider provider)
      ToChar      Method     char IConvertible.ToChar(System.IFormatProvider provider)
      ToDateTime  Method     datetime IConvertible.ToDateTime(System.IFormatProvider provider)
      ToDecimal   Method     decimal IConvertible.ToDecimal(System.IFormatProvider provider)
      ToDouble    Method     double IConvertible.ToDouble(System.IFormatProvider provider)
      ToInt16     Method     int16 IConvertible.ToInt16(System.IFormatProvider provider)
      ToInt32     Method     int IConvertible.ToInt32(System.IFormatProvider provider)
      ToInt64     Method     long IConvertible.ToInt64(System.IFormatProvider provider)
      ToSByte     Method     sbyte IConvertible.ToSByte(System.IFormatProvider provider)
      ToSingle    Method     float IConvertible.ToSingle(System.IFormatProvider provider)
      ToString    Method     string ToString(), string ToString(string format), string ToString(System.IFormatProvider pro...
      ToType      Method     System.Object IConvertible.ToType(type conversionType, System.IFormatProvider provider)
      ToUInt16    Method     uint16 IConvertible.ToUInt16(System.IFormatProvider provider)
      ToUInt32    Method     uint32 IConvertible.ToUInt32(System.IFormatProvider provider)
      ToUInt64    Method     uint64 IConvertible.ToUInt64(System.IFormatProvider provider) 
      
      
       PS C:\Users\pyelgoi> $a = "this is a string"
       PS C:\Users\pyelgoi> $a | get-member 
       
       You will see lot of options that you can use:
       
       PS C:\Users\pyelgoi> $a.Length
       16
       PS C:\Users\pyelgoi> $a.substring(0,5)
       this
       PS C:\Users\pyelgoi>

      
      
        
        PS C:\Users\pyelgoi> $b = "tom"
        PS C:\Users\pyelgoi> $a = "my name is $b"
        PS C:\Users\pyelgoi> $a
        my name is tom
        PS C:\Users\pyelgoi>
        
        
        PS C:\Users\pyelgoi> $b = "tom"
        PS C:\Users\pyelgoi> $a = "my name is $b"
        PS C:\Users\pyelgoi> $a
        my name is tom
        PS C:\Users\pyelgoi>
        
        PS C:\Users\pyelgoi> 12 -ne 12
        False
        PS C:\Users\pyelgoi> 12 -ne 13
        True
        PS C:\Users\pyelgoi> 12 -lt 13
        True
        PS C:\Users\pyelgoi> 12 -gt 13
        False
        PS C:\Users\pyelgoi>
        
        PS C:\Users\pyelgoi> "a" -eq "A"
        True
        PS C:\Users\pyelgoi> "a" -ceq "A" (Case equivalent)
        False
        PS C:\Users\pyelgoi> "Apple" -eq "A"
        False
        PS C:\Users\pyelgoi> "Apple" -like "A"
        False
        PS C:\Users\pyelgoi> "Apple" -like "A*"
        True
        PS C:\Users\pyelgoi>
        
        PS C:\Users\pyelgoi> "Apple" -like "*p*"
        True
        PS C:\Users\pyelgoi> "Apple" -like "*p?p*"
        False
        PS C:\Users\pyelgoi> "Apple" -like "*p?*"
        True
        PS C:\Users\pyelgoi>
        
        
        PS C:\Users\pyelgoi> "My name is prem" -match "prem"
        True
        PS C:\Users\pyelgoi> "My name is prem" -match "Prem"
        True
        PS C:\Users\pyelgoi> "My name is prem" -cmatch "Prem" (Case Match)
        False
        PS C:\Users\pyelgoi>
        
##  cmdlet

      cmdlet's are designed for powershell
      
      get-process
      get-service
      write-host "hello"
      
      
##   Alias

      PS C:\Users\pyelgoi> get-alias dir

      CommandType     Name                                               Version    Source
      -----------     ----                                               -------    ------
      Alias           dir -> Get-ChildItem


       PS C:\Users\pyelgoi> get-alias ls

      CommandType     Name                                               Version    Source
      -----------     ----                                               -------    ------
      Alias           ls -> Get-ChildItem
      
      
       PS C:\Users\pyelgoi> set-alias

       cmdlet Set-Alias at command pipeline position 1
       Supply values for the following parameters:
       Name: blah
       Value: get-childitem
       PS C:\Users\pyelgoi> blah

        PS C:\Users\pyelgoi> set-alias blah get-childitem
        
        
        PS C:\Users\pyelgoi> get-alias blah

        CommandType     Name                                               Version    Source
        -----------     ----                                               -------    ------
        Alias           blah -> Get-ChildItem

          
####  GO *[BACK](index.md)*        
        
    
    
    
    
    
    
    
