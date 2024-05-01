# Tutorial for fine-tuning LLMs

This is a tutorial for fine-tuning open source LLMs using QLoRA on your custom private data that is formatted in **raw text** for **free on Google Colab**.

🔗  <a href="https://colab.research.google.com/drive/1X51XC2phnD1epk5c1w9J0GnUO0BmrTRM?usp=sharing"> Google Colab notebook</a> &nbsp;&nbsp;&nbsp;&nbsp; 
📄  <a href="https://medium.com/polo-club-of-data-science/fine-tune-llms-for-free-on-custom-text-data-a-step-by-step-tutorial-8a4da6cc83f6"> Fine-tuning guide</a> &nbsp;&nbsp;&nbsp;&nbsp;
🧠  <a href="https://medium.com/polo-club-of-data-science/memory-requirements-for-fine-tuning-llama-2-80f366cba7f5"> Memory requirements</a> &nbsp;&nbsp;&nbsp;&nbsp;

<p align="center">
    <img src="imgs/llamaCartoon.png" alt="drawing" width="30%"/>
</p>

Open source LLMs like *Llama-2 7B chat* are useful for applications that involve conversations and **chatbot-like dialogue use cases**. However, these pre-trained models lack specific information due to knowledge cutoffs and do not have knowledge about your private data. Fine-tuning LLMs is a great way to "teach" these models your private data while keeping memory requirements low. We'll be using the data about the Hawaii wildfires in August 2023 sourced from the report of the Maui Police department found [here](https://medium.com/r?url=http%3A%2F%2Fwww.mauipolice.com%2Fuploads%2F1%2F3%2F1%2F2%2F131209824%2Fpre_aar_master_copy_final_draft_1.23.24.pdf). We've copied the data of the PDF into multiple text files without any additional formatting. This tutorial uses the Nvidia T4 GPU with **16 GB of VRAM** that is offered in the **free version of Google Colab**. We'll be using a quantization technique- **QLoRA**, for quantizing parameter weights to 4 bits to reduce memory requirements and increase training speed, ensuring that we don't reach the bottleneck memory.

## Getting started

Download the notebook [here](https://github.com/Sripal1/Fine-tuning-LLMs/blob/main/Fine_tune_LLMs_on_custom_data.ipynb) to run it locally or click [here](https://colab.research.google.com/drive/1X51XC2phnD1epk5c1w9J0GnUO0BmrTRM?usp=sharing) to load it in Google Colab. Then, run all the cells sequentially to get your fine-tuned model!

Since Llama-2 is a gated model, do the following steps to get access to the model:

  1. Create an account in HuggingFace [here](https://huggingface.co/join)
  2. Request access to the [Llama-2-7b-chat model here](https://huggingface.co/meta-llama/Llama-2-7b-chat-hf).

## Authors and Credits

[Sri Ranganathan Palaniappan](https://www.linkedin.com/in/sri-ranganathan-palaniappan/), CS undergrad student at Georgia Tech.

[Mansi Phute](https://www.linkedin.com/in/mansi-phute-413744166/),  CS masters student at Georgia Tech

[Seongmin Lee](https://www.linkedin.com/in/seongmin-lee-8b8a97209/),  CS PhD student at Georgia Tech

[Polo Chau](https://www.linkedin.com/in/polochau/),  Associate Professor at Georgia Tech.

## Contact
If you have any questions, please feel free to reach out to [Sri Ranganathan Palaniappan](mailto:spalaniappan9@gatech.edu?subject=LLM%20Fine-tuning%20tutorial) (BS CS@Georgia Tech).
