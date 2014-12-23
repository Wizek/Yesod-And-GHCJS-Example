
``` bash
gman gDebian»YesodAndGHCJSExample$ cabal clean
cleaning...
gman gDebian»YesodAndGHCJSExample$ cabal configure --ghcjs
Resolving dependencies...
Configuring YesodAndGHCJSExample-0.0.0...
gman gDebian»YesodAndGHCJSExample$ cabal build 
Building YesodAndGHCJSExample-0.0.0...
Preprocessing library YesodAndGHCJSExample-0.0.0...
[1 of 2] Compiling ClientSide       ( ClientSide.hs, dist/build/ClientSide.js_o )

ClientSide.hs:7:14: Warning:
    Defaulting the following constraint(s) to type ‘String’
      (Data.String.IsString a0)
        arising from the literal ‘"Hello World!"’ at ClientSide.hs:7:14-27
      (Show a0) arising from a use of ‘print’ at ClientSide.hs:7:8-12
    In the first argument of ‘print’, namely ‘"Hello World!"’
    In the expression: print "Hello World!"
    In an equation for ‘main’: main = print "Hello World!"
[2 of 2] Compiling Model            ( Model.hs, dist/build/Model.js_o )
Linking template haskell (ClientSide,ThRunner1)
Linking template haskell (ClientSide,ThRunner2)
^C
Model.hs:1:1:
    Exception when trying to run compile-time code:
      user interrupt
    Code: share
            [mkPersist sqlSettings, mkMigrate "migrateAll"]
            [(persistent-2.1.1:Database.Persist.Types.Base.$WEntityDef
                (persistent-2.1.1:Database.Persist.Types.Base.HaskellName
                   (packPTH "Order"))
                (persistent-2.1.1:Database.Persist.Types.Base.DBName
                   (packPTH "order"))
                (persistent-2.1.1:Database.Persist.Types.Base.$WFieldDef
                   (persistent-2.1.1:Database.Persist.Types.Base.HaskellName
                      (packPTH "Id"))
                   (persistent-2.1.1:Database.Persist.Types.Base.DBName
                      (packPTH "id"))
                   (persistent-2.1.1:Database.Persist.Types.Base.FTTypeCon
                      (Data.Maybe.Nothing) (packPTH "OrderId"))
                   persistent-2.1.1:Database.Persist.Types.Base.SqlInt64
                   []
                   ghc-prim:GHC.Types.True
                   (persistent-2.1.1:Database.Persist.Types.Base.$WForeignRef
                      (persistent-2.1.1:Database.Persist.Types.Base.HaskellName
                         (packPTH "Order"))
                      (persistent-2.1.1:Database.Persist.Types.Base.FTTypeCon
                         (Data.Maybe.Nothing) (packPTH "Int"))))
                []
                [persistent-2.1.1:Database.Persist.Types.Base.$WFieldDef
                   (persistent-2.1.1:Database.Persist.Types.Base.HaskellName
                      (packPTH "number"))
                   (persistent-2.1.1:Database.Persist.Types.Base.DBName
                      (packPTH "number"))
                   (persistent-2.1.1:Database.Persist.Types.Base.FTTypeCon
                      (Data.Maybe.Nothing) (packPTH "Int"))
                   (persistent-2.1.1:Database.Persist.Types.Base.SqlOther
                      (packPTH "SqlType unset for number"))
                   ...
                   ghc-prim:GHC.Types.True
                   persistent-2.1.1:Database.Persist.Types.Base.NoReference]
                []
                []
                []
                (containers-0.5.5.1:Data.Map.Base.fromList [])
                ghc-prim:GHC.Types.False)
               {entityFields = [persistent-2.1.1:Database.Persist.Types.Base.$WFieldDef
                                  (persistent-2.1.1:Database.Persist.Types.Base.HaskellName
                                     (packPTH "number"))
                                  (persistent-2.1.1:Database.Persist.Types.Base.DBName
                                     (packPTH "number"))
                                  (persistent-2.1.1:Database.Persist.Types.Base.FTTypeCon
                                     (Data.Maybe.Nothing) (packPTH "Int"))
                                  (persistent-2.1.1:Database.Persist.Sql.Class.sqlType (...))
                                  ...
                                  ghc-prim:GHC.Types.True
                                  persistent-2.1.1:Database.Persist.Types.Base.NoReference],
                entityId = persistent-2.1.1:Database.Persist.Types.Base.$WFieldDef
                             (persistent-2.1.1:Database.Persist.Types.Base.HaskellName
                                (packPTH "Id"))
                             (persistent-2.1.1:Database.Persist.Types.Base.DBName
                                (packPTH "id"))
                             (persistent-2.1.1:Database.Persist.Types.Base.FTTypeCon
                                (Data.Maybe.Nothing) (packPTH "OrderId"))
                             (persistent-2.1.1:Database.Persist.Sql.Class.sqlType
                                (Data.Proxy.Proxy :: Data.Proxy.Proxy Int))
                             []
                             ghc-prim:GHC.Types.True
                             (persistent-2.1.1:Database.Persist.Types.Base.$WForeignRef
                                (persistent-2.1.1:Database.Persist.Types.Base.HaskellName
                                   (packPTH "Order"))
                                (persistent-2.1.1:Database.Persist.Types.Base.FTTypeCon
                                   (Data.Maybe.Nothing) (packPTH "Int")))}]
```
