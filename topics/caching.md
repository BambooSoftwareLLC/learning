# Caching

Goals:
1. Why?
2. Where?
3. How often?

Useful YT short: https://www.youtube.com/shorts/fRyIwJPZbpM

Why not cache?
1. Increases code complexity
2. Don't want stale data
3. Memory constraints

Useful when:
1. Accessed multiple times in context-dependent timeframe

Considerations and/or questions to ask product owners:
1. How frequently is it accessed?
2. How frequently is it changed?
3. Prefetch at certain hours?
4. Tolerance for stale data?

Simple architecture can help simplify caching (ie. single instance backend can use `IMemoryCache` with confidence)
