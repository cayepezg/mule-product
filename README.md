## Tablas BD:

drop table if exists product;

create table product (

    id                  serial primary key,
    title               text not null,
    description         text,
    price               integer default 0,
    discountPercentage  numeric(18,2) default 0,
    rating              numeric(18,2) default 0,
    stock               integer default 0,
    brand               text,
    category            text,
    thumbnail           text,
    images              text
);


select stock from  product where id = 2;
