# InternshipII
Format Proposal dan Laporan Intership II, Aturan yang harus dipatuhi

1. file disimpan dalam format ber ekstensi .tex per chapter masing2

2. gambar disimpan dalam folder figures dengan namagambar

3. referensi dari google scholar,scholar.google.com

4. Setiap referensi yang diambil, maka tambahkan dan tuliskan ke dalam 
	file bernama refs.bib
   yang berisi kumpulan bibTex dari referensi nomor 3

5. Gunakan standar pengutipan yang baik dan benar

6. Gambar disebutkan di dalam artikel dengan format sesuai labelnya yaitu \ref{labelgambar}
   dan gambar diselipkan dengan menambahkan blok sintaks :
	```sh
	\begin{figure}[ht]
	\centerline{\includegraphics[width=1\textwidth]{figures/namagambar.JPG}}
	\caption{penjelasan keterangan gambar.}
	\label{labelgambar}
	\end{figure}
	
	Contoh :
	Pada gambar \ref{labelgambar} dijelaskan bahwa sistem operasi memiliki 3 versi.
	```
7. Referensi disebutkan dengan menyebutkan nama di dalam file bibtex No.4 
   contoh :
	Jika Bibtex :
	```sh
	@inproceedings{ganapathi2006windows,
	  title={Windows XP Kernel Crash Analysis.},
	  author={Ganapathi, Archana and Ganapathi, Viji and Patterson, David A},
	  booktitle={LISA},
	  volume={6},
	  pages={49--159},
	  year={2006}
	}
	```
	Maka artikel :
	Dalam sebuah artikel dari Ganapathi yang menyebutkan bahwa komputasi 
	adalah keniscayan \cite{ganapathi2006windows}.
	
	
8. Penyebutan subbab dan subsubbab diatur dengan cara 
	judul sub bab \section{nama sub bab}
	judul sub sub bab ditulis dengan \subsection{judul sub sub bab}
	judul sub sub sub bab ditulis dengan \subsubsection{Judul sub sub sub bab}
	contoh :
	```sh
	\section{Sejarah Peta}
	Perkembangan peta dunia tidak luput dari para ahli geografi dan kartografi. Peta dunia yang populer pada saat ini merupkan kontribusi dari para 
	pembuat peta sebelumnya

	\subsection{Ptolemy's}
	Ptolemy's diduga membuat peta pada abad ke 2
	```	

9. untuk list dan nomor gunakan enumerate atau itemize
	contoh :
	```sh
	berikut nama anggota kelompok
	\begin{enumerate}
	\item darso
	\item karyo
	\item doyok
	\end{enumerate}
	
	\begin{enumerate}
	\item
	This is the first item in the numbered list.

	\item
	This is the second item in the numbered list.
	\end{enumerate}

	\begin{itemize}
	\item
	This is the first item in the itemized list.

	\item
	This is the first item in the itemized list.
	This is the first item in the itemized list.
	This is the first item in the itemized list.
	\end{itemize}

	\begin{itemize}
	\item[]
	This is the first item in the itemized list.

	\item[]
	This is the first item in the itemized list.
	This is the first item in the itemized list.
	This is the first item in the itemized list.
	\end{itemize}
	```
10. spesial karakter menggunakan tanda \ didepannya
	contoh :
	```sh
	\& 
	\% 
	\$ 
	\#  
	\{ \}
	\_
	\"dalam petik\"
	`dalam petik'
	jika spesial karakter menjadi banyak atau satu baris gunakan verb
	contoh :
	\verb|%$'%&$&'%'%'%&'%|
	```
	
11. untuk tabel gunakan table , dan jangan lupa tabel di referensikan pada kalimat berdasarkan labelnya.
contoh:
	```sh
	ini merupakan contoh tabel \ref{table:contoh} ukuran kecil.
	\begin{table}[h]
	\caption{Small Table}
	\centering
	\begin{tabular}{ccc}
	\hline
	one&two&three\\
	\hline
	C&D&E\\
	\hline
	\end{tabular}
	\label{table:contoh}
	\end{table}
	```

12. untuk rumus gunakan tag equation dan di referensikan pada kalimat dengan tag ref sesuai labelnya
	contoh:
	```sh
	Rumus bola:

	a) Luas permukaan dijelaskan pada rumus \ref{eq:1}
	 \begin{equation}\label{eq:1}
	     L = 4 \pi r^2 \,
	\end{equation}
	b) Volume dijelaskan pada rumus \ref{eq:2}
	 \begin{equation}\label{eq:2}
	     V = \frac{4}{3}\pi r^3
	\end{equation}
	```
13. untuk kode program menggunakan verbatim
	```sh
	\begin{verbatim}
	a = "anu"
	b = "itu"
	c = a + b
	print(c) 
	\end{verbatim}
	```
