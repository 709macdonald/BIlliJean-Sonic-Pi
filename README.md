# BIlliJean

in_thread do
  8.times do
    sample :drum_cymbal_closed
    sample :bd_fat
    sleep 0.34
    sample :drum_cymbal_closed
    sleep 0.34
    sample :drum_cymbal_closed
    sample :drum_snare_hard
    sleep 0.34
    sample :drum_cymbal_closed
    sleep 0.34
    sample :drum_cymbal_closed
    sample :bd_fat
    sleep 0.34
    sample :drum_cymbal_closed
    sleep 0.34
    sample :drum_cymbal_closed
    sample :drum_snare_hard
    sleep 0.34
    sample :drum_cymbal_closed
    sleep 0.34
  end
end


in_thread do
  8.times do
    play :Fs3
    sleep 0.34
    play :Cs4
    sleep 0.34
    play :E4
    sleep 0.34
    play :Fs4
    sleep 0.34
    play :E4
    sleep 0.34
    play :Cs4
    sleep 0.34
    play :B3
    sleep 0.34
    play :Cs4
    sleep 0.34
  end
end

in_thread do
  4.times do
    play chord(:fs5, :minor), attack: 0.1, release: 1, cutoff: 80
    sleep 1.02
    play chord(:gs5, :minor), attack: 0.1, release: 1, cutoff: 80
    sleep 1.7
    play chord(:fs5, :minor7), attack: 0.1, release: 1, cutoff: 80
    sleep 1.02
    play chord(:gs5, :minor), attack: 0.1, release: 1, cutoff: 80
    sleep 1.7
  end
end
