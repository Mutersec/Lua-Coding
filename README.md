# Lua-Coding

Discord sunucuma beklerim 

Discord:https://discord.gg/WRWEk6jKG7

Bu kod örneği, bir dizinin elemanlarını işleme, dizi toplamını hesaplama, en büyük elemanı bulma, bir fonksiyon tanımlama ve faktoriyel hesaplama gibi gelişmiş özellikleri içermektedir. İleri düzey özelliklerle Lua dilinde daha karmaşık kodlar yazabilirsiniz.


local dizi = {10, 20, 30, 40, 50}


for i, eleman in ipairs(dizi) do
    print("Dizi elemanı " .. i .. ": " .. eleman)
end


local toplam = 0
for _, eleman in ipairs(dizi) do
    toplam = toplam + eleman
end
print("Dizi toplamı: " .. toplam)

local enBuyuk = dizi[1]
for _, eleman in ipairs(dizi) do
    if eleman > enBuyuk then
        enBuyuk = eleman
    end
end
print("En büyük eleman: " .. enBuyuk)


local function faktoriyel(n)
    if n <= 1 then
        return 1
    else
        return n * faktoriyel(n - 1)
    end
end


local sayi = 5
local sonuc = faktoriyel(sayi)
print(sayi .. "! = " .. sonuc)
