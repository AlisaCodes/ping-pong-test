# ping-pong-test
Ping Pong

class Fixnum
  define_method(:ping_pong) do
    array = []
    numbers = (0..self)
    numbers = numbers.to_a
    numbers.each() do |number|
    if number.==(0)
      array.push(0)
    elsif number.%(15).==(0)
      array.push("Ping-Pong")
    elsif number.%(3).==(0)
      array.push("Ping")
    elsif number.%(5).==(0)
      array.push("Pong")
    else
      array.push(number)
    end
  end
  array
  end
end
