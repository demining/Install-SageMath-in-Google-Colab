		
<figure class="wp-block-image"><img decoding="async" src="./Install SageMath in Google Colab - CRYPTO DEEP TECH_files/037-1-1024x576.png" alt="Install SageMath in Google Colab" class="wp-image-2669"></figure>



<hr class="wp-block-separator has-alpha-channel-opacity">



<p>In this article, we will do a fresh install&nbsp;<code>SageMath</code>in&nbsp;<code>Google Colab</code>.&nbsp;We previously published an article: “&nbsp;<strong><a href="https://cryptodeeptech.ru/install-sagemath-on-fedora/" target="_blank" rel="noreferrer noopener">Install SageMath for cryptanalysis on Fedora 64bit(10GB) Cloud Virtual Server</a></strong>&nbsp;”, but in order to continue cryptanalysis of the Bitcoin blockchain, many of our readers prefer to use&nbsp;<code>Debian</code> and,&nbsp;<code>Ubuntu</code>in contrast to&nbsp;<code>Fedora</code>.&nbsp;As far as we know,&nbsp;<code>Google Colab</code> it has been updated to&nbsp;<code>"Ubuntu 20.04.5 LTS"</code>.</p>



<blockquote class="wp-block-quote">
<p>We can check this by running the command:</p>
</blockquote>



<pre class="wp-block-code"><code>!cat /etc/lsb-release
</code></pre>



<hr class="wp-block-separator has-alpha-channel-opacity">


<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Install SageMath in Google Colab - CRYPTO DEEP TECH_files/image-21-1024x192.png" alt="Install SageMath in Google Colab" class="wp-image-2598"></figure></div>


<p>Therefore&nbsp;<code>"Ubuntu 20.04.5 LTS"</code>, the version allows us to install only <code>SageMath version 9.0, Release Date: 2020-01-01</code></p>



<p>Using the standard install command:</p>



<pre class="wp-block-code"><code>!sudo apt-get install -y sagemath-common</code></pre>



<figure class="wp-block-image"><img decoding="async" src="./Install SageMath in Google Colab - CRYPTO DEEP TECH_files/image-22-1024x120.png" alt="Install SageMath in Google Colab" class="wp-image-2599"></figure>



<blockquote class="wp-block-quote">
<p><strong>Unfortunately this version does not work properly.</strong></p>
</blockquote>



<p>For a complete cryptanalysis, we will install in&nbsp;<code>Google Colab</code> a completely new version <code>SageMath version 9.3</code></p>



<p>File:&nbsp;<a href="https://github.com/demining/CryptoDeepTools/blob/main/19SageMathGoogleColab/Install_SageMath_in_Google_Colab.ipynb" target="_blank" rel="noreferrer noopener"><strong>Install_SageMath_in_Google_Colab.ipynb</strong></a>&nbsp;we published in <code>GitHub</code></p>



<p>Let’s go to the official website:&nbsp;<strong><a href="https://colab.research.google.com/" target="_blank" rel="noreferrer noopener">https://colab.research.google.com</a></strong></p>



<blockquote class="wp-block-quote">
<p>Select the option&nbsp;<strong>“Upload notepad”</strong></p>
</blockquote>



<hr class="wp-block-separator has-alpha-channel-opacity">


<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Install SageMath in Google Colab - CRYPTO DEEP TECH_files/image-24.png" alt="Install SageMath in Google Colab" class="wp-image-2605"></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">



<blockquote class="wp-block-quote">
<p>Upload the file:&nbsp;<a href="https://github.com/demining/CryptoDeepTools/blob/main/19SageMathGoogleColab/Install_SageMath_in_Google_Colab.ipynb" target="_blank" rel="noreferrer noopener"><strong>Install_SageMath_in_Google_Colab.ipynb</strong></a></p>
</blockquote>



<hr class="wp-block-separator has-alpha-channel-opacity">


<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Install SageMath in Google Colab - CRYPTO DEEP TECH_files/image-25.png" alt="Install SageMath in Google Colab" class="wp-image-2606"></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">



<p>Now, through the utility,&nbsp;<code>wget</code>&nbsp;download&nbsp;<code>tar-file</code>:&nbsp;<a href="https://cryptodeeptech.ru/sage-9.3-Ubuntu_20.04-x86_64.tar.bz2" target="_blank" rel="noreferrer noopener"><strong>sage-9.3-Ubuntu_20.04-x86_64.tar.bz2</strong></a></p>



<pre class="wp-block-code"><code>!wget https://cryptodeeptech.ru/sage-9.3-Ubuntu_20.04-x86_64.tar.bz2
!tar -xf sage-9.3-Ubuntu_20.04-x86_64.tar.bz2</code></pre>



<figure class="wp-block-image"><img decoding="async" src="./Install SageMath in Google Colab - CRYPTO DEEP TECH_files/image-29-1024x321.png" alt="Install SageMath in Google Colab" class="wp-image-2612"></figure>



<hr class="wp-block-separator has-alpha-channel-opacity">



<blockquote class="wp-block-quote">
<p>Let’s go through the directory:</p>
</blockquote>



<pre class="wp-block-code"><code>cd SageMath/</code></pre>



<hr class="wp-block-separator has-alpha-channel-opacity">



<figure class="wp-block-image"><img decoding="async" src="./Install SageMath in Google Colab - CRYPTO DEEP TECH_files/image-32-1024x110.png" alt="Install SageMath in Google Colab" class="wp-image-2617"></figure>



<hr class="wp-block-separator has-alpha-channel-opacity">



<blockquote class="wp-block-quote">
<p>Open the panel and go to the folder: <code>SageMath</code></p>
</blockquote>



<hr class="wp-block-separator has-alpha-channel-opacity">


<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Install SageMath in Google Colab - CRYPTO DEEP TECH_files/image-34.png" alt="Install SageMath in Google Colab" class="wp-image-2619"></figure></div>


<blockquote class="wp-block-quote">
<p>Check if&nbsp;<code>Python-script:</code><strong> relocate-once.py is there</strong></p>
</blockquote>



<hr class="wp-block-separator has-alpha-channel-opacity">



<figure class="wp-block-image"><img decoding="async" src="./Install SageMath in Google Colab - CRYPTO DEEP TECH_files/image-33-1024x180.png" alt="Install SageMath in Google Colab" class="wp-image-2618"></figure>



<hr class="wp-block-separator has-alpha-channel-opacity">



<blockquote class="wp-block-quote">
<p>Run&nbsp;<code>Python-script:</code><strong> relocate-once.py</strong>&nbsp;with the command:</p>
</blockquote>



<pre class="wp-block-code"><code>!python3 relocate-once.py</code></pre>



<figure class="wp-block-image"><img decoding="async" src="./Install SageMath in Google Colab - CRYPTO DEEP TECH_files/image-35-1024x451.png" alt="Install SageMath in Google Colab" class="wp-image-2620"></figure>



<hr class="wp-block-separator has-alpha-channel-opacity">



<p><strong>All is ready!</strong></p>



<blockquote class="wp-block-quote">
<p>Now let’s run&nbsp;<code>SageMath</code> the command:</p>
</blockquote>



<pre class="wp-block-code"><code>!./sage -sh</code></pre>



<figure class="wp-block-image"><img decoding="async" src="./Install SageMath in Google Colab - CRYPTO DEEP TECH_files/image-36-1024x304.png" alt="Install SageMath in Google Colab" class="wp-image-2623"></figure>



<hr class="wp-block-separator has-alpha-channel-opacity">



<blockquote class="wp-block-quote">
<p>Let’s run the version check command:</p>
</blockquote>



<pre class="wp-block-code"><code>sage -v</code></pre>



<figure class="wp-block-image"><img decoding="async" src="./Install SageMath in Google Colab - CRYPTO DEEP TECH_files/image-37-1024x344.png" alt="Install SageMath in Google Colab" class="wp-image-2624"></figure>



<hr class="wp-block-separator has-alpha-channel-opacity">



<p><strong>All right!</strong></p>



<p>We’ve got a new version:&nbsp;<code>SageMath version 9.3, Release Date: 2021-05-09</code></p>



<hr class="wp-block-separator has-alpha-channel-opacity">



<blockquote class="wp-block-quote">
<p>Implementing the&nbsp;<a href="https://cryptodeeptech.ru/twist-attack/" target="_blank" rel="noreferrer noopener">Twist Attack</a>&nbsp;algorithm , download &nbsp;&nbsp;<code>Python-script:</code><a href="https://github.com/demining/CryptoDeepTools/blob/bbd83042e7405508cd2e646ad1b0819da0f9c58d/18TwistAttack/discrete.py" target="_blank" rel="noreferrer noopener">discrete.py</a></p>
</blockquote>



<pre class="wp-block-code"><code>wget https://raw.githubusercontent.com/demining/CryptoDeepTools/bbd83042e7405508cd2e646ad1b0819da0f9c58d/18TwistAttack/discrete.py</code></pre>



<hr class="wp-block-separator has-alpha-channel-opacity">



<figure class="wp-block-image"><img decoding="async" src="./Install SageMath in Google Colab - CRYPTO DEEP TECH_files/image-41-1024x517.png" alt="Install SageMath in Google Colab" class="wp-image-2628"></figure>



<hr class="wp-block-separator has-alpha-channel-opacity">



<blockquote class="wp-block-quote">
<p>To solve the discrete logarithm&nbsp;&nbsp;<em><code>(Pollard's rho algorithm for logarithms)</code></em>&nbsp;run&nbsp;&nbsp;<code>Python-script:</code><a href="https://github.com/demining/CryptoDeepTools/blob/bbd83042e7405508cd2e646ad1b0819da0f9c58d/18TwistAttack/discrete.py" target="_blank" rel="noreferrer noopener">discrete.py</a></p>
</blockquote>



<p>Now, to get the private key, we just need to run the command:</p>



<pre class="wp-block-code"><code>python3 discrete.py</code></pre>



<figure class="wp-block-image"><img decoding="async" src="./Install SageMath in Google Colab - CRYPTO DEEP TECH_files/image-43-1024x548.png" alt="Install SageMath in Google Colab" class="wp-image-2654"></figure>



<hr class="wp-block-separator has-alpha-channel-opacity">



<p><strong>Sage Math&nbsp;</strong><strong>9.3</strong>&nbsp;&nbsp;solve the discrete logarithm problem&nbsp;<em><code>(Pollard's rho algorithm for logarithms)</code></em></p>



<p><strong><br>Now everything is working properly!</strong></p>



<blockquote class="wp-block-quote">
<p>We received the private key to the Bitcoin Wallet in decimal format, then for cryptanalysis we need to follow the instructions of the article dedicated to&nbsp;&nbsp;<strong><a href="https://cryptodeeptech.ru/twist-attack/" target="_blank" rel="noreferrer noopener">Twist Attack</a></strong></p>
</blockquote>



<hr class="wp-block-separator has-alpha-channel-opacity">



<p><strong><a href="https://github.com/demining/Install-SageMath-in-Google-Colab" target="_blank" rel="noreferrer noopener">Source</a></strong></p>



<p><strong><a href="https://t.me/cryptodeeptech" target="_blank" rel="noreferrer noopener">Telegram: https://t.me/cryptodeeptech</a></strong></p>



<p><strong><a href="https://youtu.be/DBu0UnVe0ig" target="_blank" rel="noreferrer noopener">Video: https://youtu.be/DBu0UnVe0ig</a></strong></p>



<p><strong><a href="https://cryptodeeptech.ru/install-sagemath-in-google-colab" target="_blank" rel="noreferrer noopener">Source: https://cryptodeeptech.ru/install-sagemath-in-google-colab</a></strong></p>



<hr class="wp-block-separator has-alpha-channel-opacity">



<figure class="wp-block-image"><img decoding="async" src="./Install SageMath in Google Colab - CRYPTO DEEP TECH_files/037-1-1024x576.png" alt="Install SageMath in Google Colab" class="wp-image-2669"></figure>
	</div><!-- .entry-content -->
