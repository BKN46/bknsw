# 字符串工具

```lua
-- 字符串是否以某个字符串开头
function startsWith(str, start)
    return str:sub(1, #start) == start
end

-- 将a字符串按照b分割为表
function split(a, b) if b == nil then b = "%s" end
    local c = {}
    for d in string.gmatch(a, "([^" .. b .. "]+)") do table.insert(c
            , d)
    end
    return c
end
```
