```sql
CREATE table public.new AS
( SELECT * FROM public.actor limit 10)

CREATE table public.new2 AS
(SELECT A.*,C.city
FROM public.new AS a
JOIN public.city AS c ON c.city_id = a.actor_id
)
SELECT * FROM public.new2 limit 10
```

<pre>
CREATE table public.new AS
( SELECT * FROM public.actor limit 10)

<b>CREATE</b> <em>table</em> public.new2 AS
(SELECT A.*,C.city
FROM public.new AS a
JOIN public.city AS c ON c.city_id = a.actor_id
)
SELECT * FROM public.new2 limit 10
</pre>


