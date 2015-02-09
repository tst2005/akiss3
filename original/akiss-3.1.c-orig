/*

Архив рубрики: C#
AKISS 3.1
Добавить комментарий

Fast and easy to use PRNG.

Key features:

    2.5 times faster than SSE2 Mersenne’s twister
    Platform and language independent
    Period is bigger than 2^64

*/

public sealed class AKISS
{
    ulong _a = 0x6cd2d2bab6fb1b, _b = 0x42fc73c2ace698ad, _c = 0x2b20cc237775d265;
    public ulong NextUlong()
    {
        _a = _b + ((_a << 7) | (_c >> 57));
        _b = _c ^ ((_c << 13) | (_a >> 51));
        return _c = _a - ((_b << 17) | (_b >> 44));
    }
}

/*
Запись опубликована Сентябрь 4, 2012 автором admin в рубрике C#, programming с метками C#, RNG.
*/

