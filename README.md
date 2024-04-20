# Lab 8
[Fork](https://docs.github.com/en/get-started/quickstart/fork-a-repo) this repo and clone it to your machine to get started!

## Team Members
- Kaelyn Cho

## Lab Question Answers

Question 1: What is the phone number dialed in sample3.py?

Answer: 505-503-4455

Question 2: Describe your algorithm. Explain what each of these functions do: get_peak_frqs(), get_max_frq(), and get_number_from_frq().

Answer: 
decode.py iterates through the fft array and takes slices corresponding to each of the 10 tones. On each slice it performs FFT on it and splits it into the 0-1000Hz and 1000-2000Hz ranges using get_peak_frqs(). get_peak_frqs() then calls get_max_frq() which finds the frequency components of each tone by finding the maximum values within the ranges passed to it 0-1000Hz and 1000-2000Hz. Finally, get_number_from_frq() uses a dictionary to determine the number or symbol that corresponds to the combination of frequency components present in the tone. The values are concatenated into a string called output which stores the whole phone number that the tones make up.
