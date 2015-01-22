---
layout: post
title: "List Comprehensions"
description: ""
categories: [Lessons, Lists]
tags: []
---

{% include JB/setup %} 
Using a `for loop` could be useful for generating list comprehensions:
	
	isOdd = []

Algo del buen Schrödinger:

<math xmlns="http://www.w3.org/1998/Math/MathML" display="block">
  <mrow>
    <mo>[</mo>
    <mo>&#x2212;<!-- − --></mo>
    <mfrac>
      <msup>
        <mi class="MJX-variant">&#x210F;<!-- ℏ --></mi>
        <mn>2</mn>
      </msup>
      <mrow>
        <mn>2</mn>
        <mi>m</mi>
      </mrow>
    </mfrac>
    <mfrac>
      <msup>
        <mi mathvariant="normal">&#x2202;<!-- ∂ --></mi>
        <mn>2</mn>
      </msup>
      <mrow>
        <mi mathvariant="normal">&#x2202;<!-- ∂ --></mi>
        <msup>
          <mi>x</mi>
          <mn>2</mn>
        </msup>
      </mrow>
    </mfrac>
    <mo>+</mo>
    <mi>V</mi>
    <mo>]</mo>
  </mrow>
  <mi mathvariant="normal">&#x03A8;<!-- Ψ --></mi>
  <mo>=</mo>
  <mi>i</mi>
  <mi class="MJX-variant">&#x210F;<!-- ℏ --></mi>
  <mfrac>
    <mi mathvariant="normal">&#x2202;<!-- ∂ --></mi>
    <mrow>
      <mi mathvariant="normal">&#x2202;<!-- ∂ --></mi>
      <mi>t</mi>
    </mrow>
  </mfrac>
  <mi mathvariant="normal">&#x03A8;<!-- Ψ --></mi>
</math>




Y acá va un producto cruz:

<math xmlns="http://www.w3.org/1998/Math/MathML" display="block">
  <msub>
    <mrow class="MJX-TeXAtom-ORD">
      <mi mathvariant="bold">V</mi>
    </mrow>
    <mn>1</mn>
  </msub>
  <mo>&#x00D7;<!-- × --></mo>
  <msub>
    <mrow class="MJX-TeXAtom-ORD">
      <mi mathvariant="bold">V</mi>
    </mrow>
    <mn>2</mn>
  </msub>
  <mo>=</mo>
  <mrow>
    <mo>|</mo>
    <mtable rowspacing="4pt" columnspacing="1em">
      <mtr>
        <mtd>
          <mrow class="MJX-TeXAtom-ORD">
            <mi mathvariant="bold">i</mi>
          </mrow>
        </mtd>
        <mtd>
          <mrow class="MJX-TeXAtom-ORD">
            <mi mathvariant="bold">j</mi>
          </mrow>
        </mtd>
        <mtd>
          <mrow class="MJX-TeXAtom-ORD">
            <mi mathvariant="bold">k</mi>
          </mrow>
        </mtd>
      </mtr>
      <mtr>
        <mtd>
          <mfrac>
            <mrow>
              <mi mathvariant="normal">&#x2202;<!-- ∂ --></mi>
              <mi>X</mi>
            </mrow>
            <mrow>
              <mi mathvariant="normal">&#x2202;<!-- ∂ --></mi>
              <mi>u</mi>
            </mrow>
          </mfrac>
        </mtd>
        <mtd>
          <mfrac>
            <mrow>
              <mi mathvariant="normal">&#x2202;<!-- ∂ --></mi>
              <mi>Y</mi>
            </mrow>
            <mrow>
              <mi mathvariant="normal">&#x2202;<!-- ∂ --></mi>
              <mi>u</mi>
            </mrow>
          </mfrac>
        </mtd>
        <mtd>
          <mn>0</mn>
        </mtd>
      </mtr>
      <mtr>
        <mtd>
          <mfrac>
            <mrow>
              <mi mathvariant="normal">&#x2202;<!-- ∂ --></mi>
              <mi>X</mi>
            </mrow>
            <mrow>
              <mi mathvariant="normal">&#x2202;<!-- ∂ --></mi>
              <mi>v</mi>
            </mrow>
          </mfrac>
        </mtd>
        <mtd>
          <mfrac>
            <mrow>
              <mi mathvariant="normal">&#x2202;<!-- ∂ --></mi>
              <mi>Y</mi>
            </mrow>
            <mrow>
              <mi mathvariant="normal">&#x2202;<!-- ∂ --></mi>
              <mi>v</mi>
            </mrow>
          </mfrac>
        </mtd>
        <mtd>
          <mn>0</mn>
        </mtd>
      </mtr>
    </mtable>
    <mo>|</mo>
  </mrow>
</math>

Y un poco de estadística:

<math xmlns="http://www.w3.org/1998/Math/MathML" display="block">
  <mi>P</mi>
  <mo stretchy="false">(</mo>
  <mi>E</mi>
  <mo stretchy="false">)</mo>
  <mo>=</mo>
  <mrow class="MJX-TeXAtom-ORD">
    <mrow>
      <mo>(</mo>
      <mfrac linethickness="0">
        <mi>n</mi>
        <mi>k</mi>
      </mfrac>
      <mo>)</mo>
    </mrow>
  </mrow>
  <msup>
    <mi>p</mi>
    <mi>k</mi>
  </msup>
  <mo stretchy="false">(</mo>
  <mn>1</mn>
  <mo>&#x2212;<!-- − --></mo>
  <mi>p</mi>
  <msup>
    <mo stretchy="false">)</mo>
    <mrow class="MJX-TeXAtom-ORD">
      <mi>n</mi>
      <mo>&#x2212;<!-- − --></mo>
      <mi>k</mi>
    </mrow>
  </msup>
</math>

