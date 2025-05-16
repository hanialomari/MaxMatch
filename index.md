---
layout: project_page
permalink: /

title: Maximal Matching Matters Preventing Representation Collapse for Robust Cross-Modal Retrieval
authors:
    Hani Alomari, Anushka Sivakumar, Andrew Zhang, Chris Thomas
affiliations:
    Virginia Tech
paper: https://2025.aclweb.org/
##video: https://www.youtube.com/results?search_query=turing+machine
code: https://github.com/hanialomari/MaxMatchs
##data: https://huggingface.co/docs/datasets
---

<p style="margin-top: -4.75rem; text-align: center; font-weight: bold;">Paper and code will be released soon. Stay tuned!</p>

<!-- Using HTML to center the abstract -->
<div class="columns is-centered has-text-centered">
    <div class="column is-four-fifths">
        <h2>Abstract</h2>
        <div class="content has-text-justified">
Cross-modal image-text retrieval is challenging because of the diverse possible associations between content from different modalities. 
Traditional methods learn a single-vector embedding to represent semantics of each sample, but struggle to capture nuanced and diverse possible relationships cross-modally. Set-based approaches, which represent each sample with multiple embeddings, offer a promising alternative in that they can capture richer, more diverse relationships. 
In this paper, we show that, despite their promise, these set-based representations continue to face issues including sparse supervision and set collapse, which limits their effectiveness. 
To address these challenges, we propose a Maximal Pair Assignment Similarity function to optimize one-to-one matching between embedding sets which preserves semantic diversity within the set. We also introduce two loss functions to further enhance the representations: Global Discriminative Loss to enhance distinction among embeddings, and Intra-Set Divergence Loss to prevent collapse within each set. Our method achieves state-of-the-art performance on MS-COCO and Flickr30k without relying on external data.
        </div>
    </div>
</div>

<!-- After Abstract -->
<div class="columns is-centered has-text-centered">
    <div class="column is-four-fifths">
        <figure>
            <img src="fig_main.jpg" alt="Main method figure">
                <figcaption class="has-text-justified is-size-7"><em>
                    An overview of the model architecture inspired by <a href="https://arxiv.org/pdf/2211.16761" target="_blank">[Kim et al., 2023]</a>, consisting of a visual encoder, textual encoder, and set prediction modules for \( f^V \) and \( f^T \). Local and global features from each modality are processed to generate embedding sets \( S^V \) and \( S^T \), enabling more expressive cross-modal representations. We propose three core components to enhance diversity and prevent collapse: Maximal Pair Assignment Similarity, Global Discriminative Loss, and Intra-Set Divergence Loss. The Global Discriminative Loss encourages separation between individual embeddings and the global set embedding to prevent collapse, while the Intra-Set Divergence Loss enforces distinctiveness among embeddings within each set.
                </em></figcaption>
        </figure>
    </div>
</div>
---