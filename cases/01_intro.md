!SLIDE
# <span class='underscored'>3) Užitečná</span> #

!SLIDE
# Problém: více telefoních číslel #
## Typická řešení ##

!SLIDE
    @@@ SQL
    CREATE TABLE phonys (name VARCHAR, 
    phone VARCHAR);
    # Pro "více" čísel
    CREATE TABLE phonyys (name VARCHAR, 
    phones VARCHAR);

!SLIDE
    @@@ SQL
    # Pro opravdové labužníky
    SELECT phones FROM phonyys WHERE ...
    # ...
    <phones>
        <work>123-456-789</work>
        <home>987-654-321</home>
    </phones>

!SLIDE
# Správný non-Postgres postup #

Další tabulka a spárování přes cizí klíče

!SLIDE
# Postgres postup je ale něco extra #

Ustupte, přichází ...

!SLIDE bullets incremental
# hstore #

* Datový typ
* Key - value
* Bezeschémovost

!SLIDE bullets incremental
# hstore FAQ #

* Indexace?
* Lepší než XML?
* Lepší než cizí klíče?

