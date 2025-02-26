package br.com.eanassu.crudspringboot.controller;

import java.util.List;

import org.springframework.ui.Model;
import org.springframework.web.bind.annotation.GetMapping;
import org.springframework.web.bind.annotation.RequestMapping;
import org.springframework.web.bind.annotation.RestController;

import br.com.eanassu.crudspringboot.dao.FuncionarioDao;
import br.com.eanassu.crudspringboot.pojo.Funcionario;

@RestController
@RequestMapping("/funcionarios")
public class FuncionariosController {

	private FuncionarioDao dao = new FuncionarioDao();
	@GetMapping
	public String getList(Model model) {
		List<Funcionario> funcionarios = dao.getLista();
		model.addAttribute("funcionarios", funcionarios);
		return "funcionarios-list";
	}

}
