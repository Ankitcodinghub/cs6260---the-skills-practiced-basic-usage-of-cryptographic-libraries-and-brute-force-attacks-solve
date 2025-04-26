# cs6260---the-skills-practiced-basic-usage-of-cryptographic-libraries-and-brute-force-attacks-solve
**TO GET THIS SOLUTION VISIT:** [cs6260 – The skills practiced: basic usage of cryptographic libraries and brute-force attacks. Solve](https://www.ankitcodinghub.com/product/cs6260-the-skills-practiced-basic-usage-of-cryptographic-libraries-and-brute-force-attacks-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;105955&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;1&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (1 vote)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;cs6260 - The skills practiced: basic usage of cryptographic libraries and brute-force attacks. Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (1 vote)    </div>
    </div>
Digital Signature Algorithm (DSA) Key-Recovery from Nonce

Let’s recall DSA signature.

– There are public parameters (p,q,g), where p and q are large primes; p − 1 is a multiple of q and g is a group generator. Also, H(·) is a cryptographic hash function.

– Key generation KeyGen generates secret key , and public key y ← gx mod p, and outputs (x,y).

– Signing Sign(m):

– generate a random nonce k ←$ Z∗q.

– .

– output pair (r,s).

What is the vulnerability?

It is possible that the PRG used by the signer is weak and as a result the range over which the random nonce k is selected is very small. If an attacker wants to retrieve the private key from the given signature (r,s) and the message m, it can exploit the fact that nonce k is generated over a small range.

How does the attack work?

The attacker has access to the message m and (r,s) pair. It can first try to recover k by brute-force the range of k (assuming it is small). Then the secrete key x can be computed from s.

Task

Assume instead of using the large set , random nonce k is selected randomly from a small set {1,2,…,216 − 1}. You are provided with an input.json file containing:

– Public parameters: (p,q,g), where |q| = 160, |p| = 1024; for simplicity we instantiate H(·) with SHA-1.

– Public key y := gx mod p

– Message m and its signature pair (r,s) signed with x and k – Hash h = SHA-1(m) in hexadecimal representation

1

2

You are expected to compute k and produce the private key x that was used to sign the message m. There is no restriction on the language nor external cryptographic library (e.g., Crypto, OpenSSL) used for your attack. Note that we run key generation algorithm independently for each student.

Collaboration &amp; Resources

No collaboration is allowed for this homework. You are allowed to look at the examples of how to use the API of the language and cryptographic libraries and json parsing on the internet.

Submission

Please submit following three files (separately, not in a zip file),

• A textfile report.txt:

(First line) [k]

(Second line) [x]

Here is an example:

29238

59732880924362433946044405794379157682704500384

• Your implementation source file: source.[*]

• A textfile README.txt:

List any external cryptographic library or json parsing library used in your source file.

Note: replace all [*] with your input.

References

[1] https://en.wikipedia.org/wiki/Digital_Signature_Algorithm

[2] NIST.FIPS.186-4 (latest) https://nvlpubs.nist.gov/nistpubs/FIPS/NIST.FIPS.186-4.

pdf
